- Attributes
	- any quantity associated with a programming construct. 
- (Syntax-directed) translation schemes
	- notation for attaching program fragments to the productions of a grammar.
	- the program fragments are executed during syntax analysis.
	- combined result of the fragment execution, in the order induced by the syntax analysis produces the translation of the program to which this analysis/synthesis process is applied.

Syntex-directed translations will be used to translate infix expr into postfix notation, to evaluate expressions, and to build syntax trees for programming constructs.



let post(x) be the postfix notation of x
- post(E) -> E, if E is a variable or constant.
- post(E_1 op E_2) -> post(E_1) post(E_2) op
- post( (E_1) ) -> post( E_1 )
Note: 
	postfix notation(and prefix) eliminates the need for parenthesis. 
	post() is also a function i made up myself, not a notation in the book.


Converting infix notation to postfix:
- post( (9-5)+2 ) 
	-> post( (9-5) ) post(2) +
	-> post(9-5) 2 +
	-> 9 5 - 2 +

- post( 9-(5+2) )
	-> post(9) post( (5+2) ) -
	-> 9 post(5+2) -
	-> 9 post(5) post(2) + -
	-> 9 5 2 + -


Evaluating postfix notation expression:
- have an empty stack
- read each character(from left to right):
	- if it is a number, push into stack
	- if it is a operator,
		- pop the number of argument items needed
		- evaluate that expression
		- push the result back into the stack
	- if no characters left, the item in the stack is the result.

- basically, read until the operator, look to the left of the operator for operands and evaluate, continue.

