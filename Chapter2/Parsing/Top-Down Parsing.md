Top-down construction of parse tree
---
1. start at the root
2. at Node N, labeled with nonterminal A, select one of the productions for A and construct children at N for the symbols in the production body
3. Find the next node at which a subtree is to be constructed, typically the leftmost(leftmost derivation) unexpanded nonterminal of the tree.

![[Screenshot 2024-05-11 at 2.25.33 PM.png]]
Some grammars can be implemented during a single left-right scan of the input string.

- Lookahead symbol:
	The current terminal being scanned.


Example:
![[Screenshot 2024-05-11 at 2.33.01 PM.png]]
terminals(bold): 
	expr, if, for, other, empty_string

non-terminals:
	stmt, optexpr

