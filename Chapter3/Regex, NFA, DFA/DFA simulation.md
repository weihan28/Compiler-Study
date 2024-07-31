![[Screenshot 2024-06-23 at 5.31.05 PM.png]]

Since in a DFA there is exactly one transition for each character for every state
```java pseudocode
s = s0;
c = nextChar();

while (c!=eof) {
	s = move(s,c);
	c = nextChar();
}
if (s is in F) return "yes";
else return "no";
```

Given a DFA:
	Time complexity to simulate = O(|x|) always.
Important! we are excluding the time to construct it right now