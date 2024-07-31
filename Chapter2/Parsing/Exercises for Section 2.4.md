![[Screenshot 2024-05-11 at 8.40.35 PM.png]]


```java
void match(t) {
	if (lookahead==t){
		lookahead = nextLookAhead;
	}
}
```

a) 
```java

void S(){
	switch(lookahead) {
	case('+'):
		match('+');
		S(); S();
		break;
	case('-'):
		match('-');
		S(); S();
		break;
	case('a');
		break;
	default:
		throw new Exception("Syntax Error");
	}
}
```

b)
```java
/**
* S->(S)S | epsilon
* gives the same grammar as 
* S->S(S)S | epsilon.
* Since before () it will always end up as
* epsilon.
**/
void S(){
	if (lookahead=='(') {
		match('('); S(); match(')'); S();
	}
}
```

c)
```java
/**
* S -> 0 R 1
* R -> 0 R 1 | epsilon
* gives the same grammar as 
* S -> 0 S 1 | 0 1
*
**/
void S() {
	if (lookahead=='0') {
		match('0'); R(); match('1');
	} else {
		throw new Exception("Syntax Error");
	}
}

void R() {
	if (lookahead=='0') {
		match('0'); R(); match('1');
	}
}
```