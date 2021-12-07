# Compiler in C

Created (from scratch) as part of the course CS F363: Compiler Construction at BITS Pilani. The language specifications are present in the PDF. 

Collaborators (listed alphabetically): Neel Shah, Shubhankar Ranade

Compiling the compiler using the makefile creates an executable called \*drumroll\* compiler.

To execute it: <br>
``` ./compiler [input_code_file] [outfile] ```

On executing in the appropriate format, you will be asked to enter a number (0-10). Here's a description of what the program will do on entering the corresponding input:

0. Break out of the loop (i.e. Exit)

1. Print the token list generated by the lexer (on the console)

2. Parse to verify the syntactic correctness of the input source code and produce parse tree (on the console)

3. Print the Abstract Syntax Tree (on the console)

4. Display the amount of allocated memory and number of nodes to each of parse tree and AST

5. Print the Symbol Table in appropriate format showing all relevant information

6. Print the list of global variables, their types and offsets

7. Print the total memory requirement (sum total of widths of all variables in the function scope) for each function

8. Print the type expressions and width of globally visible record definitions

9. Verify the syntactic and semantic correctness of the input source code <br> If the code is syntactically incorrect, reports all syntax errors.  If the code is syntactically correct, reports all type checking and semantic errors. Also prints (on the console) the total time taken by the compiler.

10. Produce assembly code (assuming there are no syntactic, semantic or type errors)