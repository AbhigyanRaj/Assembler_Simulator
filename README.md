# Assembler and Simulator for Computer Architecture

This project is an **Assembler and Simulator** developed as part of the **Computer Architecture** course. It provides functionality to convert assembly language programs into machine code (Assembler) and simulate the execution of the machine code (Simulator). The project helps understand how instructions are executed in a CPU and the interaction between memory, registers, and instructions.

---

**Made by Abhigyann**

---

## Features

### Assembler
- **Instruction Conversion**: Converts assembly code into binary machine code.
- **Syntax Validation**: Checks assembly code for syntax errors and semantic issues.
- **Error Handling**: Provides detailed error messages for debugging.
- **Custom Instruction Set**: Supports a predefined set of instructions.

### Simulator
- **Instruction Execution**: Simulates execution of machine code instructions.
- **Register and Memory Simulation**: Mimics CPU registers and memory operations.
- **Debugging Features**:
  - Step-by-step execution.
  - Inspection of register and memory states.
- **Output Display**: Shows results for operations like arithmetic, logical, and memory access.

---

### Sample Input and Ouput

```assembly
LOAD R1, 10        # Load the value 10 into register R1
ADD R1, R2         # Add the value in R2 to R1
STORE R1, 0x20     # Store the value in R1 to memory address 0x20
HALT               # Stop execution

0001 0001 0000000000001010
0010 0001 0010 000000000000
0100 0001 0000000000100000
1111 0000 0000 000000000000

---
```

## Getting Started

### Prerequisites
- A GCC compiler for C programs.
- Basic understanding of assembly language and computer architecture concepts.

### Compilation Command
To compile the assembler executable, use the following command:

```bash
gcc -o build/assembler_executable \
src/main.c \
src/memory/memory.c \
src/instructions/instructions.c \
src/registers/registers.c \
src/utils/utils.c
