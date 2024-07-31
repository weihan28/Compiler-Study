
Translation scheme := a grammar with embedded actions

A translation scheme can be formed by extending a grammar.


Syntax-directed definition
---
This syntax-directed definition builds up a translation by attaching strings as attributes to the nodes in the parse tree.
![[Screenshot 2024-05-08 at 6.19.12 PM.png]]
- '||' means the concatenation of strings.
- needs to manipulate strings for the translation.


Syntax-Directed Translation
---
an alternate transations scheme:

**Syntax-Directed Translation scheme**
	A notation for specifying a translation by attaching program fragments to the productions in a grammar.
	
- Produces the same translation incrementally, by executing program fragments.
- Does not need to manipulate strings.



**Semantic Actions**
	program fragments embedded within the production body.
	
- position of the action to be executed is enclosed by curly braces {} within the production body.
![[Screenshot 2024-05-08 at 7.07.21 PM.png]]

- semantic actions in a parse tree
![[Screenshot 2024-05-08 at 7.09.22 PM.png]]




Examples:
![[Screenshot 2024-05-08 at 7.09.22 PM.png]]
Translate expressions consisting of digits seperated by + - signs by:
- perform a left-to-right depth-frst traversal
- execute print statement when we visit the leaf


![[Screenshot 2024-05-08 at 7.49.41 PM.png]]
 - The actions prints 95-2+ when a postorder traversal of the parse tree is executed.
 - The semantic actions translate the infix expression 9-5+2 into 95-2+ by printing each character in 9-5+2 exactly once.
 - It doesnt use any storage for the translation of subexpressions.
 - The **order** in which the printing of characters occur is significant.
 - The implementation often **does not** actually construct a parse tree as long as it ensures that the semantic actions are performed as if we constructed a parse tree and then executed the actions during postorder traversal.


https://web.stanford.edu/class/archive/cs/cs143/cs143.1128/handouts/160%20Syntax-Directed%20Translation.pdf
![[Screenshot 2024-05-08 at 8.21.21 PM.png]]