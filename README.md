# code_generation

This project implements the code generation step of a custom compiler for the TINY programming language. The TINY language is a simplified language used for educational purposes, and this compiler project aims to provide a comprehensive solution for generating code from TINY source files.

Program Input
The program takes the TINY source code as input, which can be either provided through a file or hardcoded within the program. An example of the input file format can be found in input.txt.

Program Output
Symbol Table: The program outputs the symbol table containing named variables, their initial values, and the line numbers where they appear in the code.

Each variable entry includes its name, initial value (defaulted to 0 unless explicitly assigned), and line numbers where it is referenced.
Example: [Var=x][Mem=1][Line=6][Line=7][Line=20]
Syntax Tree: The syntax tree is provided, with each non-void node accompanied by its data type enclosed in square brackets.

Operators are considered of Integer type, except LessThan and Equal, which are of Boolean type.
Numbers and IDs are also considered Integer types.
Void type nodes are not printed.
Example: [ID][x][Integer], [Oper][LessThan][Boolean]
Simulation: The program simulates the compilation process as if the code is executing. It interacts with the terminal for Read and Write statements, while other operations are handled internally.

Further Notes
If a variable appears multiple times in the same line, each occurrence is recorded in the symbol table with its respective line number.
Special TINY language constructs like repeat and write statements are handled as per the provided specifications, mimicking behavior from C-based languages.
