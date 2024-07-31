![[Screenshot 2024-06-23 at 1.43.25 PM.png]]

Build Parse Tree for regex:
![[Screenshot 2024-06-23 at 1.46.06 PM.png]]
Time Complexity: O(|r|), 
	where r = sum of the no of operators and operands in regex

Algorithm rules
---
Time complexity: O(1) for each rule.

start with:
![[Screenshot 2024-06-23 at 1.44.07 PM.png]]

- for expression a
![[Screenshot 2024-06-23 at 1.45.30 PM.png]]

![[Screenshot 2024-06-23 at 1.48.48 PM.png]]
Note: 
	all NFA constructed using these rules only have one start with no incoming and one final with no outgoing.

- r = s|t
![[Screenshot 2024-06-23 at 1.49.08 PM.png]]

- r = st
![[Screenshot 2024-06-23 at 1.50.53 PM.png]]

- r = s*
![[Screenshot 2024-06-23 at 1.52.56 PM.png]]

- r = (s)
	use N(s) as N(r).


Time Complexity
---
maximum additional state of of a rule: 2 (start and end of r=s*)
maximum additional transition of a rule: 4 (the ϵ-transition in r=s*)

Since we apply each rule(O(1) time) for each operators and operands of the parse tree:
	Time complexity of REG -> NFA construction: O(|r|) x O(1) = **O(|r|)**

Worst case NFA structure:
- n = 2|r|
- m = 4|r|
	where 
		n = num of states in the final NFA
		m = num of transitions in the final NFA
		r = sum of the no of operators and operands in regex