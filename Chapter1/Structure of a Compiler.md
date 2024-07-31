![[Screenshot 2024-05-07 at 2.35.30 AM.png]]
- Main parts of compilation:
	- Analysis
	- Synthesis

- Analysis(front end of a compiler):
	- breaks up source program into constituent pieces and imposes a grammatical structure(syntax tree) on them.
	- uses this structure to create an intermediate representation of the source program.
	- provides error messages if syntax or semantic errors are found.
	- collects information about the source program and stores it in a symbol table.
	- syntax tree is also a form of intermediate representation.
	- Note: intermediate representation is just the inner representations of the source program during the compilation process that aren't the source and target program.

- Synthesis(back end of a compiler):
	- constructs the desired target program from intermediate representation and the info in the symbol table.



![[Screenshot 2024-05-07 at 2.52.33 AM.png]]
- Phases of a compiler:
	1) [[Lexical Analysis]]
	2) [[Syntax Analysis]]
	3) [[Semantic Analysis]]
	4) [[Intermediate Code Generation]]
	5) [[Code Optimisation]]
	6) [[Code Generation]]

- Symbol-Table Management
	- Records the variable names used in the source program.
	- Collects info about various attributes of each name.
	- may provide info about the storage allocated for a name, type, scope.
	- may provide in the case of procedure names, number and types of its arguments, method of passing each argument(by value or by reference) and type returned.
	- a data structure containing a record for each variable name, with fields for the attributes of the name.
	- should have quick data access and data retrieval.



Some compiler collections have been created with carefully designed intermediate representation that allow:
- the front end for a language to interface with the back end of a certain target machine.
- combining different front ends with back end for the target machine gives compilers for different source languages for one target machine.
- we can also combine a front end with different back ends for different target machines.