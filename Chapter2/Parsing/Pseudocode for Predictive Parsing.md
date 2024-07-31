Grammar for parser:
![[Screenshot 2024-05-11 at 2.33.01 PM.png]]


- match(t):
	compares its argument t with the lookahead symbol and advances to the next input terminal if they match(ie: the moving forward of the lookahead). 
	
- lookahead variable:
	a global variable that holds the currently scanned input terminal.


 ![[Screenshot 2024-05-11 at 5.42.48 PM.png]]
- for each terminal, do match(terminal)
- for each non-terminal, call terminal_procedure()
- body of the stmt prodecure:
	![[Screenshot 2024-05-11 at 5.57.07 PM.png]]



Java pseudocode for the match(t) procedure
```java
/**
* compares the lookahead and the 
* terminal being considered(t), 
* 
* move the lookahead if matching,
* raise syntax error if not.
**/
void match(t) {
	if (lookahead==t) {
		lookahead = nextTerminal;
	} else {
		report("syntax error);
	}
}
```

Java pseudocode code fot the stmt procedure:
![[Screenshot 2024-05-11 at 5.59.20 PM.png]]
```java
// pseudocode
/**
* terminals: 
* expr if for other ( ) ; 
* non-terminals:
* stmt, optexpr
**/
void stmt() {
	switch(lookahead) {
	case(expr):
		match(expr); match(';'); 
		break;
	case(if):
		match(if); match('('); match(expr);
		stmt(); 
		break;
	case(for):
		match(for); match('(');
		optexpr(); match(';');
		optexpr(); match(';');
		optexpr(); match(')'); 
		stmt(); 
		break;
	case(other):
		match(other);
		break;
	default: 
		report("syntax error")
	}
}
```

Java pseudocode code for the optexpr procedure:
![[Screenshot 2024-05-11 at 6.09.21 PM.png]]

```java
void optexpr() {
	if (lookahead==expr){
		match(expr);
	}
	// do nothing if its empty
}
```



When to use empty_string productions
---
- the pseudocode/grammar for optexpr() above uses empty_str as the default when no other productions can be used.

After matching the terminal('('), we move the lookahead to get:
![[Screenshot 2024-05-11 at 7.07.09 PM.png]]
Note: the node to consider(^) is just the procedure that is running.

we see that lookahead is not expr, so nothing happens to the lookahead. Instead the next precedure executes, giving:
![[Screenshot 2024-05-11 at 7.09.44 PM.png]]and then we continue.

Generally:
	consider a variant of the optexpr 
	where expr is a non-terminal instead.
![[Screenshot 2024-05-11 at 7.12.19 PM.png]]

if lookahead symbol not in FIRST(expr):
	use the empty_str production.