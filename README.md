# Assembler and Simulator for Computer Architecture

This project is an **Assembler and Simulator** developed as part of the **Computer Architecture** course. It provides functionality to convert assembly language programs into machine code (Assembler) and simulate the execution of the machine code (Simulator). The project helps understand how instructions are executed in a CPU and the interaction between memory, registers, and instructions.

---

**Made with ❤️ by Abhigyann**

---

## Table of Contents
1. [Features](#features)
2. [Getting Started](#getting-started)
   - [Prerequisites](#prerequisites)
   - [Compilation Command](#compilation-command)
   - [Execution Command](#execution-command)
3. [Usage](#usage)
4. [Examples](#examples)
   - [Sample Input](#sample-input)
   - [Sample Output](#sample-output)
5. [Project Structure](#project-structure)
6. [Instruction Set](#instruction-set)
7. [Contributing](#contributing)
8. [License](#license)
9. [Acknowledgments](#acknowledgments)

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
