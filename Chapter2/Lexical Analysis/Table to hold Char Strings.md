Single Representation
---
- a string table insulate the rest of the compiler from the representation of strings.
- phases of compiler can work with references or pointers to the string in the table.
- references can be manipulated more efficiently than the strings themselves.

Reserved Words
---
- initialise the string table with reserved strings and their tokens.

when lexical analyzer reads a string or a lexeme that could form a identifier:
1. Check if lexeme is in the string table, returns the token from table if it is.
2. return a token with terminal **id** otherwise.


String Table
---
- implemented using a hashtable.
```java
/**
Maps lexemes -> tokens
**/
Hashtable words = new Hashtable();
```

looking up reserved words(pseudocode):
```java
if (peek holds a letter) {
	collect letters or digits into a buffer b;
	s=string formed from characters in b;
	w=token returned by words.get(s)
	
	if (w is not null) return w;
	else {
		Enter the key-value pair <s, <id,s>> into words
		return token <id, s>;
	}
}
```