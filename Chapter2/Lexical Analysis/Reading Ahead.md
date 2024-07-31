A lexical analyzer might need to read ahead some characters to decide what token is to be returned by the parser.

Example:
	curr_char = '>'
	is it the > token or >= token.

General approach
---
maintain a input buffer which the lexical analyzer can read and push back characters.

- A pointer keeps track of the portion of the input that has been analyzed.
- pushing back a char is implemented by moving back the pointer.

One char read ahead usually suffice: variable peek
- read next char to distinguish (t,true) and (1,10)
- no read ahead needed for (\*)
- either holds the char beyond the lexeme for the char token, or it holds a blank.