- actual parameters: 
	parameters used in the call of a procedure.
- formal parameters:
	parameters used in the procedure definition.


- Call-by-Value:
	- actual parameter is evaluated(if it is an expression) or copied (if it is a variable).
	- all computation involving the formal parameters done by the procedure is local to that procedure(no side effect).
- Call-by-Reference:
	- address of the actual parameter is passed to the callee as the value of the corresponding formal parameter.
	- Uses of the formal parameter in the code of the callee are implemented by following this pointer to the location indicated by the caller.
	- Changes to the formal parameter appears as changes the actuall parameter.


Aliasing
-- 
- two formal parameters that refer to the same location are aliases of one another.
- two variables, which may appear to take their values from two distict formal parameters can become aliases of each other.
- understanding aliasing and the mechanisms that create it is essential if a compiler is to optimize a program.
- many situations where optimising is only possible if we are certain variables are not aliased.


