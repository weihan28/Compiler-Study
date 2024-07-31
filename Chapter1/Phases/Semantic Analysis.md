![[Screenshot 2024-05-07 at 3.23.12 AM.png]]
- checks for semantic consistency with language definition
- gathers **type information** and saves it in the syntax tree or symbol table for intermediate-code generation
- **type checking** occurs here, checks if each operator has matching operands. Reports an error if a float is used for array indexing etc.
- Some language specifications permit **type conversions** called **coercions**. Notice the operator **inttofloat** node that explicitly converts the integer 60 into a floating-point number 60.0.