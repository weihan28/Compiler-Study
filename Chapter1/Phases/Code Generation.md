![[Screenshot 2024-05-07 at 3.53.52 AM.png]]
- maps the intermediate representation into the target language. 
- If the target language is machine code, registers or memory locations are selected for each variables used by the program.
- A crucial aspect of this is the judicious assignment of registers to hold variables.

Machine language generated above:
- Loads the float value of id3 into register R2.
```assembly
LDF R2, id3
```
- Multiply Float value of R2 with 60.0 and store it into register R2.
```assembly
MULF R2, R2, #60.0
```
- Load the content of id2 into register R1.
```assembly
LDF R1, id2
```
- Add the float content of register R1 with register R2 and store it in R1.
```assembly
ADDF R1, R1, R2
```
- Store the float content of register R1 into the memory location of id1.