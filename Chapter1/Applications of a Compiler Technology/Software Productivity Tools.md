- data-flow analysis to locate errors along all the possible execution paths, and not just those exercised by the input data sets.
- the problem of finding all program errors is undecidable.
- Optimisers must be conservative and cannot alter the semantics of the program under any circumstances.


- Type Checking
- Bounds Checking
- Memory-management Tools
	- garbage collection, a tradeoff between efficiency and a combination of ease of programming and software reliability.
	- automatic memory management obliterates all memory-management errors, a major source of problems in C and C++.
	- Purify is a tool that dynamically catches memory management errors as they occur.