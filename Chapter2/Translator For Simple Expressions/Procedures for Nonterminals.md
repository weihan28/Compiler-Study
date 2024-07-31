Previous Translation Scheme:
![[Screenshot 2024-05-14 at 11.17.10 PM.png]]

Procedure(pseudocode):
```java

void expr() {
	term(); rest();
}

void rest() {
	if(lookahead=='+') {
		match('+'); term(); print('+'); rest();
	} else if (lookahead=='-') {
		match('-'); term(); print('-'); rest();
	} else {/*do nothing*/}
}

void term(){
	if (lookahead is a digit) {
		t = lookahead;
		match(lookahead); print(t);
	} else {
		report("syntax error");
	}
}
```