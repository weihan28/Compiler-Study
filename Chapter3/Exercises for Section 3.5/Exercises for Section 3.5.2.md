![[Screenshot 2024-06-21 at 7.48.17 PM.png]]

```lex
%{  
#include <stdio.h>  
  
FILE *fic;  
  
%}  
blank   [ \t\n]  
ws      {blank}+  
  
%%  
  
{ws}    {fprintf(fic, "%s", " ");}  
.       {fprintf(fic, "%s", yytext);}  
  
%%  
  
int main() {  
    fic = fopen("output.txt","w");  
    if (!fic) {  
        perror("Error opening file");  
        return 1;  
    }  
    yylex();  
    return 0;  
}
```

run using:
```zsh 
lex lex2.l  
gcc lex.yy.c -o lexer -ll    
./lexer < input.txt
```
Command explanation:
	lex2.l is suppose to go through a input file and write it to output.txt.  
	use the commands to run lex2.l on input.txt.  
  
- compile lex2.l into lex.yy.c: 
```zsh
lex lex2.l 
```
  
- compile lex.yy.c into an executable called lexer using the gcc c compiler with lex lib:  
```zsh
gcc lex.yy.c -o lexer -ll  
```

- direct the input file input.txt into the executable to run it as input:  
```zsh
./lexer < input.txt  
```


input.txt:
```txt
wdsrfje  
    adadadjwqe  
     sadaddas  
  
  ad1233.;';';  
  
  sasda[e]
```

output.txt(after running the commands):
```txt
wdsrfje adadadjwqe sadaddas ad1233.;';'; sasda[e]
```

Note:
running "./lexer < input.txt" does not change the output.txt output.
eof file check can be added explicitly.
```lex
<<EOF>> {return 0;} 
```