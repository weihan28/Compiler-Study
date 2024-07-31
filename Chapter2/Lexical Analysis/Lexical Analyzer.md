reads characters from input and groups them into "token objects"

- Token(in this section): a terminal along with additional info
- Lexeme: sequence of input char that comprises a single token
- Lexical analyser insulates a parser from the lexeme representation of tokens.

Note: in this section, the lexical analyser allows numbers, identifiers and "white space"(blank, tabs and new lines)

Previous syntax-directed translation(with * and / added):
![[Screenshot 2024-05-16 at 2.19.48 AM.png]]
- terminal **num** is assumed to have attribute **num**.value
- terminal **id** has a string-valued attribute written as **id**.lexeme, assume this string is the actuale lexeme comprising this instance of token **id**