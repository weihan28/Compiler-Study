Instruction sets:
- RISC(Reduced Instruction-Set Computer)
- CISC(Complex Instruction-Set Computer)
	- Originally intended to make assembly easier
	- Include complex memory-addressing modes to support data-structure accesses and procedure-invocation instructions that save registers and pass parameters on the stack.
	
	Code optimisations often can reduce these instructions to a small number of simple operations by eliminating redundancies across complex instructions.
	
	It is desirable to build simple instruction sets like RISC as the compiler can use them much more effectively and the hardware is easier to optimize.

based on RISC concept:
- PowerPC
- SPARC
- MIPS
- Alpha
- PA-RISC

based on CISC:
- x86

	however, the most effective way to use a high-performance x86 machine is to use just its simple instructions.

	many ideas from RISC are used in implementing the processor itself.


Specialized Architectures:
- data flow machines
- vector machines
- VLIW (Very Long Instruction Word)
- SIMD (Single Instruction, Multiple Data) arrays of processors
- systolic arrays
- multiprocessors with:
	- shared memory
	- distributed memory