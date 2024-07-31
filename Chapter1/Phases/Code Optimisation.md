![[Screenshot 2024-05-07 at 4.36.15 AM.png]]
- attempts to improve the intermediate code so that better target code will result.

- better could be:
	- faster
	- shorter
	- less power consumiing
	
- The image shows that the result of t1 is inlined and inttofloat is removed.

- t3 is removed since its only used once to transfer the value to id1.



Optimizing Compilers:
- compilers for optimising the intermediate code.
- a significant amount of time is spent here, so optimisations must be selected carefully.
- there are some simple optimisations that significantly improve the running time of the target program without slowing down compilation too much.