Derivation Examples
---
- CFG
![[Screenshot 2024-05-08 at 12.09.04 PM.png]]
- derivation of string "aaaa" 
![[Screenshot 2024-05-08 at 12.08.18 PM.png]]
- Parse tree of derivation
![[Screenshot 2024-05-08 at 10.59.41 AM.png]]


- CFG
![[Screenshot 2024-05-08 at 12.16.21 AM.png]]![[Screenshot 2024-05-08 at 12.16.31 AM.png]]
- Parse tree for 9-5+2
![[Screenshot 2024-05-08 at 12.11.58 PM.png]]



- Dyck language
![[Screenshot 2024-05-08 at 12.26.54 PM.png]]
- CFG
![[Screenshot 2024-05-08 at 12.27.50 PM.png]]
- Derivation
![[Screenshot 2024-05-08 at 12.28.17 PM.png]]
- Parse Tree
![[Screenshot 2024-05-08 at 12.28.38 PM.png]]



Leftmost Derivation vs Rightmost Derivation
---
- Leftmost Derivation:
	- derive the leftmost non-terminal at every step
- Rightmost Derivation:
	- derive the rightmost non-terminal at every step

CFG:
![[Screenshot 2024-05-08 at 12.31.15 PM.png]]
Parse Tree:
![[Screenshot 2024-05-08 at 12.31.57 PM.png]]



Ambiguity
---
A grammer is *ambiguous* if more than one parse tree can generate the same string of terminals.
![[Screenshot 2024-05-08 at 3.38.01 PM.png]]
Note: 
- one grammer that is ambiguous doesnt mean that all grammer for that language is ambiguous.
- but there still exists *inherently ambiguous languages* that does not have unambiguous grammar.


Associativity of Operators
---
Associativity is only needed when the operators in an expression have the same precedence.
 ![[Screenshot 2024-05-08 at 2.28.30 PM.png]]
- Left associative
	- addition, subtraction
		- 7 - 4 + 2 = ((7-4)+2)
	- multiplication, division
		- 7\*2/3 = (7\*2)/3
- Right associative
	- exponentiation(^)
		- 5^4^3^2 = 5^(4^(3^2))
	- assignment(=)
		- a=b=c is a=(b=c)
		
Grammar for right-associative operator = for strings like a=b=c.
![[Screenshot 2024-05-08 at 2.48.39 PM.png]]
Grammar for left associative operator +- for strings like 1+2-3.
![[Screenshot 2024-05-08 at 2.51.55 PM.png]]
Note: 
- right associatice recurse to the right. A -> B + A
- left associative recurse to the left. A -> A + B




Precedence of Operators
---
[relative precedence levels ](https://arc.net/l/quote/tmceqxqg)of operators found in many C-style languages
![[Screenshot 2024-05-08 at 2.24.26 PM.png]]
![[Screenshot 2024-05-08 at 2.25.20 PM.png]]
![[Screenshot 2024-05-08 at 2.27.04 PM.png]]