- peek: variable that stores the next input character
- line: variable that stores the number of lines until now

skipping white space(pseudocode)
```java
for (;;peek=next_input_char) {
	if(peek is ' ' or '\t') {do nothing}
	else if (peek is '\n') {line += 1}
	else break;
}
```


skips all blank and tab, increment line if next line.