Abstract Syntax Tree
---
![[Screenshot 2024-05-14 at 9.58.03 PM.png]]
- Nodes: operator
- Leafs: value
- No helper nodes unlike parse tree(like terms and factors.)


different to a parse tree, parse trees are sometimes calles a concrete syntax tree, and the underlying grammar is a concrete syntax for the language.

It is desirable for a translation scheme to be based on a grammar whose parse trees are as close to syntax trees as possible.
Example: 
![[Screenshot 2024-05-14 at 10.05.40 PM.png]]
This syntax-directed translation scheme has grouping of subexpressions that are similar to the grouping in syntax trees.
subexpression of addition are given by expr and term.