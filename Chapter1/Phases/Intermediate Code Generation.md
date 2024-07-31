![[Screenshot 2024-05-07 at 3.41.25 AM.png]]
- many compilers generate an explicit low-level or machine-like intermediate representation.
- This intermediate representation should be 
	- easy to produce
	- translate into the target machine.

Example:
![[Screenshot 2024-05-07 at 3.48.16 AM.png]]
- Three-Address Code
	- a sequence of assembly-like instructions with max 3 operands per instruction.
	- each operant acts like a register.
	- at most 1 operator on the right side
	- temporary name(id1) must be generated to hold the result computed.
