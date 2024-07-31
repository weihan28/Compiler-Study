![[Screenshot 2024-06-23 at 5.35.32 PM.png]]
	Initial is construction, per string is simulating on x.
if the regular expression is only one time use like grep, converting NFA further to DFA is not needed. 

For a lexical analyser that uses the same regex for lots of simulations, DFA is preferred.

Mixed strategy:
![[Screenshot 2024-06-23 at 5.40.08 PM.png]]
when we simulate NFA, and we run the "on the fly" subset construction, we get the set of states which represent the states reachable after reading one c and multiple or no ϵ (S_new) from another set of states(S_old), which is exactly what the c column for DFA row S_new represents.
	ie: row S_old in Dstates for column c is S_new.
	we can memoize this to use it for later S_olds.






Why DFA has a worst case structure of 2^|r| number of states.
 the num of states of a DFA can range from:
- typical DFA: s = |r|, 
	time = O(r^3)
	might not be worth it if FA is only one time use.
- worst case DFA(rare in practice): s = 2^|r|,
	time = O((2^|r|)(r^2))
	in this case, space and time is too much.

https://courses.engr.illinois.edu/cs374/fa2018/notes/models/DFAproofs.pdf

since the highest worst space complexity(which also causes its time complexity for construction to be exponential too) is exponential growth O(a^n),
if we find any example of this time complexity, which they do, it means that it acts as a suitable upper bound for all DFA's.
![[Screenshot 2024-06-23 at 5.54.21 PM.png]]
same but instead of using binary it uses a and b.
this DFA has a minimum of 2^n states.

so there exist a DFA with the maximum of exponantial time and space complexity for construction.
meaning DFA can go up to 2^n time and space complexity for construction.