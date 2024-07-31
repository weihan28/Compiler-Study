![[Screenshot 2024-06-14 at 1.02.23 PM.png]]
![[Screenshot 2024-06-14 at 1.40.48 PM.png]]
Exercise 2.8.1:
```java
class For extends Stmt {
	Expr init; Expr cond; Expr inc;
	Stmt s;
	public For(Expr init, Expr cond, Expr inc, Stmt s) {
		this.init = init;
		this.cond = cond;
		this.inc = inc;
		this.s = s;
	}

	public void gen() {
		Label start = newlabel();
		Label after = newlabel();
		// generate(emits) inter code for the initialisation expr(Assign)
		init.gen();
		// put a label to signify start of equivalent while loop 
		emit(start + ":");
		Expr c = cond.rvalue();
		emit("ifFalse" + c.toString() + " goto " + after);
		s.gen();
		inc.gen(); // emit(generate) code for increment
		emit("goto " + start);
		// end of while loop
		emit(after + ":");
	}
}
```
![[Screenshot 2024-06-14 at 1.40.57 PM.png]]
Exercise 2.8.2:

- C uses 0 and 1 to represent true and false instead.
- instead of checking "ifFalse" we can check "ifZero" or "ifEqual" 0 instead.

replace:
```java
emit("ifFalse" + c.toString() + " goto " + after);
```

with:
```java
emit("ifZero" + c.toString() + " goto " + after);
// or
emit("ifEqual" + c.toString() + " 0 goto " + after);
```