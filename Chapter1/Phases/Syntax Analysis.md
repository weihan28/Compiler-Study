or *parsing*

![[Screenshot 2024-05-07 at 3.17.16 AM.png]]
- Uses the token stream produced by the lexical analizer to create a tree-like intermediate representation that depicts the grammatical structure.
- A typical representation is a syntax tree, each interior node represent an operation and the children of the node represent the arguments.
- Precedence is reflected in the syntax tree, multiplication is performed before addition.


- Context-free grammars:
	- help specify the grammatical structure as the language 
	- used to discuss algorithms for constructing efficient syntax analyzers automatically from certain classes of grammars.
- Syntax-directed definitions:
	- help specify the translation of prog language constructs.