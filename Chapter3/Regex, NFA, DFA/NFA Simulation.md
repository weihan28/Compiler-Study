Given inputs:
- **NFA** N (from regex->nfa construction), 
	with start state s0, accepting states F, transition func *move*
- input string **x**,
	terminated with **eof** character

Note: NFA construction from r takes O(|r|) time.

![[Screenshot 2024-06-23 at 2.19.40 PM.png]]

strategy: smt like "on the fly" **subset construction** 
	idea is to keep track of all the possible routes that can be taken by using the char read as input, and ϵ-transitions only.

Note: 
	subset construction for DFA runs for each state of DFA and each possible character, while this only runs for the char read until it reaches eof.


```java pseudocode

S = ϵ-closure(s0); // starting point
c = nextChar();
while (c is not eof) {
	S = ϵ-closure(move(S, c));
	c = nextChar();
}

if (S ∩ F ≠ Ø)  // S contains one or more Final States.
	return "yes";
else
	return "no";
```


Note: move(S) uses O(|S|) time, since it uses the NFA transition table and fetches for each s in S. if s is just 1 state, its O(1).

ps: creating the transition table prolly just takes O(n|∑|) time.
![[Screenshot 2024-06-23 at 4.36.05 PM.png]]

Recursive Implementation (efficient)
---
![[Screenshot 2024-06-23 at 4.13.11 PM.png]]

```java pseudocode
/* oldStates and newStates and c 
(global variables for util func to mutate and access) */
S_old = new Stack();
S_new = new Stack();
c = nextChar();

// Initialisation: uses the normal ϵ-closure(s0).
for each s in ϵ-closure(s0) {
	S_old.add(s);
}

while (c!=eof) {
	updateS(c);
	c = nextChar();
}

if (S ∩ F ≠ Ø)  // S contains one or more Final States.
	return "yes";
else
	return "no";
```
utility functions
```java pseudocode
/* gets S_new after reading c and ϵ from S_old 
resets the boolean array and swaps S_new and S_old when finish

implements:
S = ϵ-closure(move(S, c));
*/
updateS() {
	while (S_old is not empty) {
		s = S_old.pop();
		for (t on move[s,c]) 
			if (!alreadyOn[t])
				addState(t); // handles ϵ-closure(t)(modified)
	}

	while (S_new is not empty) {
		s = S_new.pop();
		S_old.push(s);
		alreadyOn[s] = false;
	}
}
```
```java pseudocode
/*DFS(recursive approach) but only traversing ϵ-transition and states NOT inside newStates*/
addState(s) {
	newState.push(s); 
	alreadyOn[s] = True; 
	for (t on move[s,ϵ])
		if (!alreadyOn[t]) 
			addState(t);
}
```

Time Complexity
--
suppose NFA N has,
	n states, m transitions

for updateS(excluding addState):
```java pseudocode
/* Implements:
S = ϵ-closure(move(S, c));
*/
updateS() {
	while (S_old is not empty) { // O(n)
		s = S_old.pop();
		// for (t on move[s,c]) is just part of the DFS
			// if (!alreadyOn[t]) 
				// addState(t); excluding addState
	}

	while (S_new is not empty) { // O(n)
		s = S_new.pop();
		S_old.push(s);
		alreadyOn[s] = false;
	}
}
```
Total Time Complexity of updateS for each c(excluding addState) = O(2n)
Total Time Complexity of updateS for each c(including addState) = O(3n+m)

for addState:
```java pseudocode
updateS() {
..
for (t on move[s,c]) 
	if (!alreadyOn[t]) 
		addState(t); 
..
}

addState(s) {
	newState.push(s); 
	alreadyOn[s] = True; 
	for (t on move[s,ϵ])
		if (!alreadyOn[t]) 
			addState(t);
}
```

We know that we only call addState if s/t is not in alreadyOn, hence:
- we at most call addState on all states exactly once: O(n) calls
- the total aggregate iterations for the two for loops are at maximum
	m times, where we loop for every edge.

Total Time Complexity of addState for each c = O(n+m)
	which is the how the time complexity of DFS is infered.

Total Time Complexity of NFA Simulation
==

```java pseudocode
S_old = new Stack();
S_new = new Stack();
c = nextChar();

for each s in ϵ-closure(s0) { // O(n)
	S_old.add(s);
}

while (c!=eof) { // O(k=|x|)
	updateS(c);  // O(3n+m)
	c = nextChar();
}

// O(|min(S,F)|)=O(n) max, if we loop through
if (S ∩ F ≠ Ø)  
	return "yes";
else
	return "no";
```
Given inputs:
- **NFA** N (from regex->nfa construction), 
	with start state s0, accepting states F, transition func *move*
- input string **x**,
	terminated with **eof** character

we can check if NFA accepts the input x in:
	O(n) + O(k(3m+n)) + O(n) = O(k(m+n))
	where k = |x|

Worst case structure of NFA:
- n = 2|r|
- m = 4|r|

Simulating NFA (excluding construction):
O(|x| (2|r|+4|r|)) = O( |x| x |r|)
the size of input + size of regex!

Since Constructing NFA takes O(|r|):
	the total time for constructing and simulating a regex takes:
	O(|x| x |r|) + O(|r|) = O( |x| x |r|)





















Iterative implementation (and why it sucks)
---
Note: this is what i came up with myself, might be just skill issue or incorrect

Problems:
- super complicated, unreadable and error prone
- t on ϵ-closure(move[s,c]) also returns the states that are in newStates.
	since it initialises res = all t∈T, and move also gives states that are already on newStates.
```java psueudocode
oldStates // states that act as starting points
newStates // temporary storage for new states after reading c
alreadyOn = [false]*(n+1) // tells if a state s is in newStates

initialise oldStates = ϵ-closure(s0); // too time consuming
// newStates contains new states discovered in ϵ-closure(s0)

while (c!=eof) {

	while (oldStates is not Empty) {
		s = oldState.pop();
		for (t on ϵ-closure(move[s,c])) 
			if (!alreadyOn[t]) // if t is not already reachable
				newStates.push(t);
				alreadyOn[t] = true;
	}
	
	while (newStates is not Empty) {
		s = newStates.pop();
		alreadyOn[s] = false;
		oldStates.push(s);
	}
}

/** Now only discovers and traverses new states(doesn't discover a state twice, unless it is alrdy inside T)
*/
ϵ-closure(T) {
	discovered = all t∈T; // stack
	res = all t∈T;
	// normal ϵ-closure on the oldState (starting point)
	while (discovered is not Empty) {
		s = discovered.pop();
		alreadyOn[s] = True;

		// each ϵ-transition of s->t.
		for (each t in move[s,ϵ]) {
			if (!alreadyOn[t]) {
				discovered.push(t);
			}
		}
	}
	return res;
}


..// check for return "yes" or "no"
```