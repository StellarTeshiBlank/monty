# Goal: 
This project is to create an interpreter for Monty ByteCodes Files

## Monty ByteCode Files
* The Monty byte codes usually have the .m extension. 
* Most of the industry uses this standard but it is not required by the specification of the language. There is not more than one instruction per line. There can be any number of spaces before or after the opcode and its argument
* Monty byte code files can contain blank lines (empty or made of spaces only. and any additional text after opcode or its requred argument is not taken into account:
* Usage: monty file
	- where file is the path to the file containing Monty byte code
* If the user does not give any file or more than one argument to your program, print the error message USAGE: monty file, followed by a new line, and exit with the status EXIT_FAILURE
* If, for any reason, it's not possible to open the file, print the error message Error: Can't openfile <file>, followed by a new line, and exit with the status EXIT_FAILURE
 	- where is the line number where the instruction appears.
	- Line numbers always start at 1
* The monty program runs the bytecodes line by line and stop if either:
	- It executed properly every line of the file
	- It finds an error in the file
	- an error occured
* If you can't malloc anymore, print the error message Error:malloc failed, followed by a new line, and exit with status  EXIT_FAILURE.
* You have to use malloc and free and are not allowed to use any other function from man malloc (realloc, calloc,...)

### This is tested on Ubuntu 20.04 LTS
### compiled with C - gcc -Wall -Werror - Wextra -pedantic -std=c89 *.c -o monty

### Project done by Manuchimso Egwurugwu
