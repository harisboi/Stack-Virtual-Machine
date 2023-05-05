# Stack-Based Virtual Machine

This project provides an example of building a simple stack-based virtual machine from scratch using C++. The virtual machine reads in a file containing bytecode instructions and executes them, using a stack to store intermediate results.

## Prerequisites

To run this virtual machine, you will need:

- A C++ compiler that supports C++17
- A command-line interface

## Building and Running

To build the virtual machine, clone this repository and run the following commands:

cd stack-vm
make


This will compile the source code and create an executable file called stack-vm.

To run the virtual machine, use the following command:

/stack-vm <filename>


Replace `<filename>` with the name of the file containing bytecode instructions. The virtual machine will read in the instructions, execute them, and print the result.

The supported opcodes and operands are:

- `push <value>`: Pushes a value onto the stack.
- `add`: Pops the top two values off the stack, adds them, and pushes the result onto the stack.
- `sub`: Pops the top two values off the stack, subtracts them, and pushes the result onto the stack.
- `mul`: Pops the top two values off the stack, multiplies them, and pushes the result onto the stack.
- `div`: Pops the top two values off the stack, divides them, and pushes the result onto the stack.
- `mod`: Pops the top two values off the stack, computes the remainder, and pushes the result onto the stack.
- `pop`: Pops the top value off the stack and discards it.
- `print`: Prints the top value on the stack.
