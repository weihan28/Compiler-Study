Depth-first traversal:
![[Screenshot 2024-05-08 at 6.51.14 PM.png]]

Bottom-up traversal:
	evaluates attributes at a node after having evaluated attributes at its children.

- syntax-directed definition does not impose a specific order for the evaluation of attributes on a parse tree.
- Synthesized attributes can be evaluated during any bottom-up traversal.
- with both synthesized and inherited attributes, the matter of evaluation order is quite complex.


Preorder and Postorder Traversals
---
both are special cases of depth-first traversals.
![[Screenshot 2024-05-08 at 6.57.42 PM.png]]