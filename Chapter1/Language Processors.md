![[Screenshot 2024-05-07 at 1.42.22 AM.png]]
![[Screenshot 2024-05-07 at 1.45.38 AM.png]]
1) Compiler:
	- translates a source language into a target language.
	- if target program is an executable machine-language program, it can be called by the user to process input and produce outputs


![[Screenshot 2024-05-07 at 1.46.43 AM.png]]
2) Interpreter:
	- executes the operations of the source program with the input and produces an output.



Pros of a Compiler over Interpreter:
- target program produced by compiler is usually faster at mapping inputs to outputs.
Pros of a Interpreter over Compiler:
- gives better error diagnostics, since it executes the source program statement by statement.



![[Screenshot 2024-05-07 at 1.55.27 AM.png]]
Java language processors:
- combines compilation and interpretation(hybrid compiler)
- java source program -> bytecodes-> interpreted by virtual machine.
- bytecodes compiled can by interpreted on another machine, perphaps across a network.
- some java compilers, called "just-in-time" compilers translate bytecodes into machine language immediately before running the intermediate program to process the input. This gives faster processing of input to output.



![[Screenshot 2024-05-07 at 2.07.12 AM.png]]
Other programs working with the coompiler:
- Preprocessor:
	- A source program might be divided into modules stored in seperate files.
	- collecting and generating the source program is done by the preprocessor.
	- also expands shorthands(macro) into source language statements.

- Assembler:
	- If a compiler produces assembly-language as the target language, it will be processed by the assembler afterwards.
	- Processes assembly and produces relocatable machine code as output.
	- Having assembly as target language is easier to produce and debug.

- Linker:
	- Resolves external memory addresses, where the code in one file may refer to a location in another file.
	- Large programs are often compiled in pieces, relocatable machine code may have to be linked together with other relocatable object files and library fles into code that actually runs on the machine.
	- Hands it to Loader afterwards.

- Loader:
	- puts together all of the executable object files into memory for execution.


Exercises:
- Exercise 1 . 1 . 1 : What is the difference between a compiler and an interpreter? 
	- A compiler translates a source program of a source language into a target program with a target language.
	- A interpreter instead of translating takes in a source program and input and executes the source program statement by statement to produce an output.
	
- Exercise 1 . 1 . 2 : What are the advantages of (a) a compiler over an interpreter (b) an interpreter over a compiler?
	- Target programs produced by compilers are usually faster at mapping input to outputs than interpreters.
	- Interpreter gives better error diagnostic since it executes the source program statement by statement.
	
- Exercise 1.1.3: What advantages are there to a language-processing system in which the compiler produces assembly language rather than machine language?
	- Assembly is easier to produce and debug.

- Exercise 1.1.4 : A compiler that translates a high-level language into another high-level language is called a source-to-source translator. What advantages are there to using C as a target language for a compiler?
	- C is a language that has fast compilation time and execution time compared to the original source language.
	
- Exercise 1 . 1 . 5 : Describe some of the tasks that an assembler needs to per­ form.
	- Processes Assembly to produce relocatable machine code.