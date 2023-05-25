###Monty

###Glamour Maphanga's Monty Project Readme:

###This repository contains the Monty project, which is a simple interpreter for Monty bytecode files. The project is implemented in C.

###Project Overview

***The Monty project implements a stack-based interpreter for Monty bytecode files. The interpreter supports various operations such as pushing elements onto the stack, printing stack values, performing arithmetic operations, manipulating the stack, and more.

***Monty is a simple interpreter for Monty Bytecode files. Monty Bytecode files have the .m extension and contain a series of opcodes that can be executed by the Monty interpreter.

###Installation
***To use Monty, follow these steps:

###Clone the Monty repository from GitHub:

***$ git clone https://github.com/username/monty.git

###Navigate to the repository directory:

***$ cd monty

###Compile the source code using the provided Makefile:

***$ make

###This will generate an executable file named monty.

###Usage
###To run a Monty Bytecode file, use the following command:

***$ ./monty <filename>

###Replace <filename> with the path to the Monty Bytecode file you want to execute.

###Supported Opcodes
###Monty currently supports the following opcodes:

***push <int>: Pushes an element to the stack. The <int> argument must be an integer. If it's not, an error message is printed.

###Example: push 1

***pall: Prints all the values on the stack, starting from the top of the stack.

###Example:
push 1
push 2
push 3
pall
###Output:
3
2
1
***pint: Prints the value at the top of the stack.

***pop: Removes the top element of the stack.

***swap: Swaps the top two elements of the stack.

***add: Adds the top two elements of the stack. The result is stored in the second top element, and the top element is removed.

***nop: No operation, does nothing.

***sub: Subtracts the top element of the stack from the second top element. The result is stored in the second top element, and the top element is removed.

***div: Divides the second top element of the stack by the top element. The result is stored in the second top element, and the top element is removed. If the top element is 0, an error message is printed.

***mul: Multiplies the second top element of the stack with the top element. The result is stored in the second top element, and the top element is removed.

***mod: Computes the rest of the division of the second top element of the stack by the top element. The result is stored in the second top element, and the top element is removed. If the top element is 0, an error message is printed.

***pchar: Prints the character represented by the ascii value at the top of the stack.

***pstr: Prints the string starting at the top of the stack. The stack elements are treated as ascii values until a 0 or an ascii value outside the valid range is encountered.

***rotl: Rotates the stack to the top. The top element becomes the last one, and the second top element becomes the first one.

***rotr: Rotates the stack to the bottom. The last element becomes the top element.

***stack: Sets the format of the data to a stack (LIFO). This is the default behavior of the program.
The queue opcode sets the format of the data to a queue (FIFO).

###When switching to the queue mode:

***The top of the stack becomes the front of the queue.
***The front of the queue becomes the top of the stack.
#endif
