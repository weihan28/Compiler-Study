Applies to any grammar that has disjoint FIRST sets for the production bodies belonging to any nonterminal.

The procedure for nonterminal A does 2 things:

First:
 - decides which production to use by examining the lookahead symbol.
 - The production with body a(where a is not empty_str) is used if lookahead in FIRST(a).
 - If there is a conflict with 2 nonempty bodies for a lookahead then this method cannot be used. Example: 
	 A -> a and A->b, 
	 lookahead is in both FIRST(a) and FIRST(b).
- if A has emp_str production, then it is only used when the lookahead symbol is not in the FIRST set for any other production body of A.

Second:
- mimics the body of the chosen production. That is, the symbols of the bode are "executed" in turn from the left.
- nonterminals are "executed" by a call to its corresponding procedure.
- terminals that match the lookahead are "executed" by reading the next input symbol. 
- If at any point a terminal in the body doesnt match with the lookahead a syntax error is reported.



Constructing a syntax-directed translator from a predictive parser
---
1. Construct a predictive parser, ignor the actions in the productions.
2. Copy the actions from the translation scheme into the parser. Note the placement of the action in the code of the body. 



Left Recursion
---
"left-recursive" productions like this causes the recursive-descent parser to loop forever.
![[Screenshot 2024-05-11 at 8.15.45 PM.png]]
- the leftmost symbol of the bode is the same nonterminal at the head of the production.

	If the procedure expr decides to apply this production for a lookahead, it calls expr() again WITHOUT moving the lookahead.
	Hence, with the same lookahead, the same production is called and it loop forever.
- Left-recursion can be eliminated by rewriting the offending production.

Left/RIght-recursive productions
---
![[Screenshot 2024-05-11 at 8.20.53 PM.png]]
- nonterminal A and its production are *left recursive*.
- One of its production has A itself as the leftmost symbol on the right side.
- Applies the first production one or more times to append 1 or more alphas towards the left, and finally one B.

The same effect can be achieved by rewriting the productions for A in the following mannar, using a new non-terminal R:
![[Screenshot 2024-05-11 at 8.33.11 PM.png]]
- This grammer is right recursive that produces the same output.
- Applies the B first and then adding one or more alphas to the right.

![[Screenshot 2024-05-11 at 8.30.34 PM.png]]
- Left-recursive productions lead to trees that grow down towards the left.
- Right-recursive productions lead to trees growing down towards the right.
- Trees growing down to the right make it harder to translate expressions containing left-associative operators.