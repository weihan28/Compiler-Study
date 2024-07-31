or *scanning*

![[Screenshot 2024-05-07 at 2.54.10 AM.png]]
- Reads the stream of characters making up the source program and groups the characters into lexemes. 
- For each Lexeme the lexical analyser produces as output a token.
- char_stream -> lexemes -> tokens

![[Screenshot 2024-05-07 at 2.49.57 AM.png]]	
- Token:
	- PS: Token class with name and value attribute.
	- stored in the symbol table.


Example:
- Character stream
![[Screenshot 2024-05-07 at 2.57.53 AM.png]]

| Lexeme   | Token         | abstract symbol used |
| -------- | ------------- | -------------------- |
| position | <id, 1>       | id : identifier      |
| =        | <=>           | = : assignment       |
| initial  | <id, initial> | id : identifier      |
| +        | <+>           | + : addition         |
| rate     | <id, rate>    | id : identifier      |
| *        | <*>           | * : multiplication   |
| 60       | <60>          |                      |
Note: Blanks are discarded

- Final sequence of tokens
![[Screenshot 2024-05-07 at 3.07.14 AM.png]]






![[Screenshot 2024-05-07 at 2.52.33 AM.png]]