Previously:
![[Screenshot 2024-05-14 at 11.28.05 PM.png]]

1) Eliminate Tail Recursion using iteration: 
	recursive calls at end of body are replaced with iteration.
```java
void rest() {
	while(true) {
		if(lookahead=='+') {
			match('+'); term(); print('+'); continue;
		} else if (lookahead=='-') {
			match('-'); term(); print('-'); continue;
		} else {/*do nothing*/}
		break;
	}
}
```

2) Inline *rest()* into *expr()* since it is the only call of expr in the whole procedure
```java

void expr() {
	term();
	while(true) {
		if(lookahead=='+') {
			match('+'); term(); print('+'); continue;
		} else if (lookahead=='-') {
			match('-'); term(); print('-'); continue;
		} else {/*do nothing*/}
		break;
	}
}

/* no more rest()*/

void term(){
	if (lookahead is a digit) {
		t = lookahead;
		match(lookahead); print(t);
	} else {
		report("syntax error");
	}
}
```