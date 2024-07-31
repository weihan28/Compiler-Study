**Subset Construction**
---
![[Screenshot 2024-06-23 at 1.33.40 AM.png]]
![[Screenshot 2024-06-23 at 3.26.43 AM.png]]
![[Screenshot 2024-06-23 at 2.55.10 AM.png]]
![[Screenshot 2024-06-23 at 2.44.05 AM.png]]
```java pseudocode
/** generates the DFA transition table for a given NFA */
Dstates.add( ϵ-closure(s0) );

while (there is a unmarked(not yet processed) state T in Dstate){
	for (each input alphabet c like a,b) {
		DState U = ϵ-closure(move(T, c));
		if (U not in Dstates)
			Dstate.add(U); // U is unmarked
		Dtran(T, c) = U;  // fill in the table
	}
	mark T; // as calculated
}
```
Time Complexity: s x a x O(m+n) = O(sa(m+n))
	where
		s = num of states of final **DFA**,
		n = num of states in NFA,
		m = num of transition of NFA, 
		a = len(∑), ie the num of input alphabets of DFA

Later we will see that for the NFA constructed from reg expression has:
- at most 2|r| states
- at most 4|r| transitions
- at most |r| input symbols
	Total time comp constructing DFA trans table from NFA 
		= O(s x |r| (|4|r| + 2|r||)) = **O(sr^2)**
		where |r| stands for the size of the regex that the NFA is constructed from (the sum of the number of operators and operands in r)

and the num of states of a DFA can range from:
- typical DFA: s = |r|, 
	time = O(r^3)
	might not be worth it if FA is only one time use.
- worst case DFA(rare in practice): s = 2^|r|,
	time = O((2^|r|)(r^2))
	in this case, space and time is too much.

ϵ-closure(T) or ϵ-closure(s)
---
for a set of states T:
	give all states that is reachable by any t∈T only using ϵ-transitions.

essentially DFS run with all t from T in stack, and only traversing ϵ-transitions.
![[Screenshot 2024-06-23 at 3.12.24 AM.png]]
```java pseudocode
/* gives all states reachable only using 0 or more ϵ-transitions from
any t∈T */
ϵ-closure(T) {
	stack = all t∈T;  // discovered stack
	res = all t∈T;

	while (stack is not empty) {
		t = stack.pop();
		for (each outgoing ϵ-transitions from t to v) {
			if (v not in stack) {
				stack.push(v);
				res.add(v);
			}
		}
	}
	return res;
}
```

Worst Time Complexity: O(n + m)
	where 
		n=num of states of NFA
		m = num of transition of NFA 
- ie: normal DFS time : O(V+E)
NOTE: 
- its n because we might need to at most discover every state in the NFA.
- its m because the number of ϵ-transitions is at most m. 
	ie: a NFA that is entirely consisting of ϵ-transitions, with all states reachable from T.