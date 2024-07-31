function *scan* that returns token objects
```java
Token scan() {
	skip white space, as in 2.6.1;
	handle numbers, as in 2.6.3;
	handle reserved words and identifiers, as in 2.6.4;
	/* if we get here, treat read-ahead character peek as a token*/
	Token t = new Token(peek);
	peek = blank /* initialisation, as in 2.6.2 */*
	return t;
}
```

package **lexer** has classes tokens and a class **Lexer** containing function **scan**
![[Screenshot 2024-05-27 at 10.03.48 PM.png]]
- tag: used for parsing decisions
- value: integer value
- lexeme: used for reserved words and identifiers

Token class:
```java
package lexer;

public class Token {
	public final int tag;
	public Token(int t) { 
		tag = t; 
	}
}
```
- takes in a tag attribute

a new object of class Token with integer representation of '+'
```java
new Token('+')
```

Tag class:
```java
package lexer;

public class Tag {
	public final static int
		NUM = 256, ID = 257, TRUE = 258, FALSE = 259;
}
```
- defines named constants, like python's enum.
- Tag.NUM and Tag.ID refers to terminals **num**, **id**
- reserved word uses their own tag, while named variables/identifiers use ID tag.


Num class, extends Token class:
```java
package lexer;

public class Num extends Token {
	public final int value;
	public Num(int v) {
		super(Tag.NUM);
		value = v;
	}
}
```
- Num uses Tag.Num as its tag


Word class, extends Token class:
```java
package lexer;

public class Word extends Token {
	public final String lexeme;
	public Word (int t, String s) {
		super(t);
		lexeme = new String(s);
	}
}
```
- word takes in a tag t as int
- word is used for reserved word and identifiers, so it expects a integer tag value.
- a reserved word can be created using 
```java
new Word(Tag.TRUE, "true")
```


Code for lexical analyzer, part 1 of 2
```java
package lexer;
import java.io.*;
import java.util.*;

public class Lexer {
	public int line = 1;
	private char peek = ' ';
	private Hashtable words = new Hashtable();

	public Lexer() {
		// reserved word uses their own tag
		reserve( new Word(Tag.TRUE, "true") );
		reserve( new Word(Tag.FALSE, "false") );
	}

	void reserve(Word t) {
		words.put(t.lexeme, t);
	}

	public Token scan() throws IOException {
		/*
		scan sequence of blank/tab/newline
		- do nothing if blank or tab
		- increment line for newline
		*/
		for ( ; ; peek = (char)System.in.read() ) {
			if ( peek == ' ' || peek == '\t' ) continue;
			else if (peek == '\n' ) line = line + 1;
			else break;
		}
		/* continues later*/
	}
}
```
- reserved words are initialised before the first call of scan
- peek is initialised as blank ' '

continuation
```java
package lexer;
import java.io.*;
import java.util.*;

public class Lexer {
	public int line = 1;
	private char peek = ' ';
	private Hashtable words = new Hashtable();

	public Lexer() {
		reserve( new Word(Tag.TRUE, "true") );
		reserve( new Word(Tag.FALSE, "false") );
	}

	void reserve(Word t) {
		words.put(t.lexeme, t);
	}

	/**
	Scans and returns the next Token.
	Token is either Num/Word/just a token(symbol) otherwise, like token('+')
	*/
	public Token scan() throws IOException {
		/*
		scan sequence of blank/tab/newline
		- do nothing if blank or tab
		- increment line for newline
		*/
		for ( ; ; peek = (char)System.in.read() ) {
			if ( peek == ' ' || peek == '\t' ) continue;
			else if (peek == '\n' ) line = line + 1;
			else break;
		}
		
		/*
		scan sequence of digit to form Num
		- if next char(peek) is digit, add it to v.
		*/
		if ( Character.isDigit(peek) ) {
			int v = 0;
			do {
				v = v*10 + Character.digit(peek, 10);
				peek = (char)System.in.read();
			} while ( Character.isDigit(peek) );
			return new Num(v);
		}
		
		/*
		scan sequence of characters to form string
		- if next char(peek) is char, add it to b
		*/
		if ( Character.isLetter(peek) ) {
			StringBuffer b = new StringBuffer();
			do {
				b.append(peek);
				peek = (char)System.in.read();
			} while ( Character.isLetterOrDigit(peek) );
			String s = b.toString();
			// check to see if it is reserved word
			Word w = (Word)words.get(s);
			if ( w != null ) return w;
			// construct and add new word if not
			w = new Word(Tag.ID, s);
			words.put(s, w);
			return w;
		}

		/*
		just returns the token with peek as tag
		if it is not a letter, digit, blank,tab,newline
		*/
		Token t = new Token(peek);
		peek = ' ';
		return t;
	}
}
```

![[Screenshot 2024-05-28 at 11.55.51 AM.png]]

pg90