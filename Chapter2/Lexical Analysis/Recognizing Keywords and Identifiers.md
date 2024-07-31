most languages use fixed char strings such as **for**, **do**,**if** as punctuation marks or to identify constructs.

Character Strings are used as **identifiers** to **name** variables, arrays, functions etc.

Grammars routinely treat identifiers as terminals to simplify the parser, which can just expect the same terminal, say **id** each time any identifier appears in the input.

Input:
![[Screenshot 2024-05-27 at 6.31.05 PM.png]]

parser works with terminal stream: **id = id + id**

Token for **id** has attribute that holds the lexeme.
![[Screenshot 2024-05-27 at 6.32.21 PM.png]]

Keywords vs Identifiers:
	keywords generally also satisfy rules for forming identifiers.
- Mechanism is needed to decide if a lexeme forms a keyword or identifier.
- problem easier resolved if keywords are *reserved*. Making character strings that are not a keyword an identifier.
- *reserved*: cannot be used as identifiers.

