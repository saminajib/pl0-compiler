# PL/0 Compiler


## Description

    This project is an implementation of a Recursive Descent Parser and Intermediate
    Code Generator for the programming language PL/0. It builds off of the lexical analyzer
    that takes in the source code and tokenizes it. If a program does not follow the correct
    grammar conventions of PL/0, then a message will be outputted indicating the type
    of error present. This project uses the full PL/0 grammar rather than just a subset.

---------------------------------------

## Compilation Instructions

    Compile the code in eustis using command "gcc hw4compiler.c"

---------------------------------------

## Usage

    Run the compiled code using "./a.out [arguments]"
    Sample inputs are given: input0.txt, etc.

    # It is assumed that the argument for this program should be a .txt file
    # containing a program written in PL/0.

---------------------------------------

## Example

    Example command:
        ./a.out input.txt

    Expected output:
        Should output the PL/0 program source code and then corresponding assembly instructions, as
        well as a file called elf.txt containing the assembly code that can be run in the VM.
        If there is an error, then only a message indicating the type of error that has occurred
        will be outputted.

---------------------------------------

# Virtual Machine

## Description

    This project is an implementation of a virtual machine called the P-machine.
    It is a stack machine that has one memory area called the process address
    space (PAS). The PAS is divided into 3 segments: the first 10 locations, called
    "unused", the "text", which contains the instructions for the VM to execute
    and the "stack", which is organized as a data-stack to be used by the PM/O CPU.

---------------------------------------

## Compilation Instructions

    Compile the code in eustis using command "gcc vm.c"

---------------------------------------

## Usage

    Run the compiled code using "./a.out [arguments]"

---------------------------------------

## Example

    Example command:
        ./a.out elf.txt

    Expected output:
        Result of processing the commands inside of input.txt

---------------------------------------