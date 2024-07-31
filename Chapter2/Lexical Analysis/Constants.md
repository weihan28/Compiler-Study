Integer constants can be allowed either by
- creating a terminal symbol, **num** or
- incorporating the syntax of integer constants into the grammar

Input "31 + 28 + 59" is transformed into
![[Screenshot 2024-05-27 at 6.24.24 PM.png]]

Pseudocode for grouping digits into integers:
```java
if (peek holds a digit) {
	v=0;
	do {
		v=v*10 + integer value of digit peek
		peek = next input character
	}
	return token <num, v>
}
```