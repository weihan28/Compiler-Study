Grammar for arithmatic expressions
---
- start with the 4 common arithmatic operators:
	+, -, \*, /
	
- precedence table:
	operator on the same line have same associativity and precedence.
![[Screenshot 2024-05-08 at 2.32.20 PM.png]]



- create 2 nonterminals *expr* and *term* for 2 levels of precedence. 
	- A extra *factor* for generating basic units in expressions.
	- basic units are presently digits and parenthesized expressions.
![[Screenshot 2024-05-08 at 2.34.40 PM.png]]
	Note: factors cannot be seperator when placed beside other operators.



- Consider the binary operators \* and /, that have the highest precedence. 
	- Accociate to the left, so productions are similar for lists that associate to the left.
		![[Screenshot 2024-05-08 at 2.51.55 PM.png]]
![[Screenshot 2024-05-08 at 2.47.45 PM.png]]



- similar construction for binary operators + and -, which associate to the left.
![[Screenshot 2024-05-08 at 2.56.30 PM.png]]



- Resulting grammar
![[Screenshot 2024-05-08 at 2.57.46 PM.png]]



Generalisation of the expression grammar above.
---
![[Screenshot 2024-05-08 at 2.59.06 PM.png]]
- factor: 
	- expression that remains always whole when an higher precedence operator is placed beside it.
	- 1+2 is not an factor, since 1+2\*3 tears the 2 away from the expression.
	- (1+2) is a factor, 2^(1+2) still has (1+2) as a single expression.
	- Note: any parenthesized expr here is a factor.

- term(that is not also a factor):
	- expression that can be torn apart by operators of higher precedence, but not by lower-precedence operators.
- expression(that is not a term or factor):
	- can be torn apart by any operator.

- n precedence levels need n+1 nonterminals.
	![[Screenshot 2024-05-08 at 2.34.40 PM.png]]
	- first is factor, that cannot be torn apart. Typically has a body of single operand and parenthesized expression.
	
	![[Screenshot 2024-05-08 at 3.13.55 PM.png]]
	- for each other level, there is 1 nonterminal representing expressions that an be torn apart only by operators at that level or higher. Typically, the productions for this nonterminal have bodies representing uses of the operators at that level, plus one body that is just the nonterminal for the next higher level.



Keywords
---
- allow recognition of statements
- most statements begin with a keyword or a special character. Exceptions include assignments and procedure calls.
- statements defined by (ambiguous) grammer for java, production for expression not shown.
- java allows a=b=c, but the grammar bellow does not.
- placement for semicolons (;) should be placed carefully. 
![[Screenshot 2024-05-08 at 3.24.33 PM.png]]