# Code-2

//Write the entire process of compilation of a .c file to .exe file. Show and verify each process step by step by terminal commands.

1. Preprocessing:This command runs the preprocessor on program.c, expanding macros, including header files, and performing other preprocessing tasks. The output is stored in program.i.
Command: gcc -E program.c -o program.i
Verification: Open program.i in a text editor to see the expanded code.
2. Compilation:This command compiles the preprocessed code in program.i into assembly language instructions, storing the result in program.s.
Command: gcc -S program.i -o program.s
Verification: Open program.s in a text editor to view the assembly code.
3. Assembling:This command assembles the assembly code in program.s into machine code, generating an object file named program.o.
Command: gcc -c program.s -o program.o
Verification: You can use a tool like objdump or a hex editor to examine the contents of the object file.
4. Linking:This command links the object file program.o with any necessary library files to create the final executable file program.exe.
Command: gcc program.o -o program.exe
Verification: Run the executable from the command line: ./program.exe

