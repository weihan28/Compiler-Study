![[Screenshot 2024-06-15 at 4.03.06 PM.png]]
C language
---
https://www.gnu.org/software/gnu-c-manual/gnu-c-manual.html#Identifiers
i) sets of char that form the input alphabet(excluding those inside strings and comments)
```txt
Letters: Upper and Lower
- Upper: [A-Z]
- Lower: [a-z]

digits: [0-9]

character constants: 
(most are only used inside strings, except whhitespace)
- backslash: '\\'
- question mark: '\?'
- single quotation mark: '\''
- double quotation mark: '\"'
- audible alert: '\a'
	beeps when outputted
- backspace: '\b'
- esc(GNU extension): '\e'
- form feed(page-break): '\f'
- newline: '\n'
	goes to next line with carriage return
- carriage return: '\r'
	returns the print head back to the beginning
- horizontal tab: '\t'
- vertical tab: '\v'
	goes to the next line without carriage return
- octal number(octal escape sequence): '\o', '\oo', '\ooo'
    o is any valid octal digit. up to only 3 after backslash
	"\779"-> '\77' and '9'
	77(base 8, octal) = 63(decimal)
	ascii(63) = '?'
	output of print("\779") is "?9"
- hexadecimal(hex escape sequence): '\xh', '\xhh', '\xhhh', ...

whitespace: (can be used to seperate tokens)
- ' ', '\t', '\n', '\v', '\f'

Special Characters and Symbols:
- Punctuation: ,.:?-_()[]{}#@$%^&*-+<>|\/~
- String/Char delimiters: " '
```

ii) lexical form of numerical constants
```txt
Integer Constants
----
decimal:
- not prefixed: 1, 0, 123, -456
hexadecimal:
- prefixed with 0(x|X): 0xF12, 0XFFF
octal:
- prefixed with 0: 076, 017

Forcing int constant to be long/unsigned by appending
unsigned integer type: (u|U)
long integer type: (l|L)

unsigned int: 45U
unsigned long: 45UL, 45LU

Real Number Constants
----
4.7, -4.7, .7, 38., 5e-2, 5e2, 6.022E23

append letter to cause it to a type, if no letters type is double.
float: (F|f)
ling: (l|L)
```
iii) lexical form of identifiers
```txt
used for naming cariables, functions, new data types and preprocessor macros.

can include letters, decimal digits, underscore
- first char cannot be a digit.
- case sensitive.
- '$' only allowed in GNU extensions.

_df23, foo, FOO, _12df1
```



C++ language
---
https://learn.microsoft.com/en-us/cpp/cpp/character-sets?view=msvc-170
i) sets of char that form the input alphabet(excluding those inside strings and comments)
![[Screenshot 2024-06-15 at 5.29.16 PM.png]]

ii) lexical form of numerical constants
```txt
Integer literals
----

decimal integral literal:
Dddd..(d=[1-9],d=[0-9]): 154, 234

octal integral literal:
0ooo..(o=[0-7]): 0123, 077

hexadecimal integral literal:
0(x|X)hh..(h=[0-F]): 0xFF2, 0X3FFF

suffixes for integer literals:
unsigned (u|U): 328U
long(l|L): 328L
long long(ll|LL): 328LL

0x8000000ULL

digit seperators(no effect on compilation):
24'847'458'121
```

![[Screenshot 2024-06-15 at 5.43.29 PM.png]]![[Screenshot 2024-06-15 at 5.43.54 PM.png]]

iii) lexical form of identifiers
![[Screenshot 2024-06-15 at 5.47.04 PM.png]]
![[Screenshot 2024-06-15 at 5.46.02 PM.png]]



C\#
---
https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/



Fortran
---
fortran 77:
https://docs.oracle.com/cd/E19957-01/805-4939/index.html
i) sets of char that form the input alphabet(excluding those inside strings and comments)
![[Screenshot 2024-06-15 at 6.00.07 PM.png]]![[Screenshot 2024-06-15 at 6.00.27 PM.png]]
![[Screenshot 2024-06-15 at 6.00.47 PM.png]]


ii) lexical form of numerical constants
![[Screenshot 2024-06-15 at 6.09.16 PM.png]]
![[Screenshot 2024-06-15 at 6.10.10 PM.png]]

iii) lexical form of identifiers
![[Screenshot 2024-06-15 at 6.17.14 PM.png]]
![[Screenshot 2024-06-15 at 6.17.31 PM.png]]
