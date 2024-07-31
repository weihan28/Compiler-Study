![[Screenshot 2024-06-21 at 10.18.00 PM.png]]

```lex
/* Exercise 3.5.4 */  
  
%{  
    #include <stdio.h>  
  
    FILE *fic;  
%}  
  
vowel       [Aa]|[Ee]|[Ii]|[Oo]|[Uu]|[Yy]  
consonant   [B-Db-dF-Hf-hJ-Nj-nP-Tp-tV-Xv-xZz]  
letter      [A-Za-z]  
  
%%  
  
{consonant}{letter}*    {fprintf(fic, "%s%c%s", yytext+1, yytext[0], "ay");}  
{vowel}{letter}*        {fprintf(fic, "%s%s", yytext, "ay");}  
.                       {fprintf(fic, "%s", yytext);}  
[\n]                    {fprintf(fic, "%s", yytext);}  
  
%%  
  
int main() {  
    fic = fopen("output.txt", "w");  
    if (!fic) {  
        perror("Error opening file");  
        return 1;  
    }  
    yylex();  
    return 0;  
}
```

input.txt:
```lex
123 aasddadz  
    badaasdasd .  asd
```

output.txt:
```lex
123 aasddadzay  
    adaasdasdbay .  asday
```