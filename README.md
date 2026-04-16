# Shaw Recursive Function (P06)

An x86 Assembly Language (MASM) program that implements a recursive function called `shaw(n)`. 

The function follows specific rules based on the input value `n` and demonstrates proper recursion techniques, stack frame management, and register preservation.

**Author:** DN MBOYI  
**Student Number:** 222019179  
**Subject:** CSC03B3  
**Practical:** P06  
**Year:** 2025  

---

## Problem Description

The program asks the user to enter a number `n` between **0 and 100**. It then computes `shaw(n)` using the following recursive rules:

- If `n ≤ 0`: return **1**
- If `0 < n ≤ 5`: return `n << 1` (i.e., `n * 2`)
- If `n ≥ 6`: return `shaw(n >> 3) + shaw(n - 3)`

The program validates the input (must be between 0 and 100 inclusive), displays an error message for invalid inputs, and allows the user to run multiple calculations until they choose to exit.

---

## Features

- **Recursive Function** (`shaw PROC`) with three distinct cases
- Proper **stack frame** setup using EBP
- Correct parameter passing and stack cleanup (`RET 4`)
- Register preservation (`PUSHFD` / `POPFD` and general registers)
- Input validation (0 to 100)
- Clear error handling for out-of-range inputs
- Formatted output showing the computed result
- Loop support for multiple test cases

---

## Technologies Used

- **x86 Assembly Language**
- **MASM** (Microsoft Macro Assembler)
- **Recursion** with stack-based calls
- **io.inc** library for input/output

---

## How to Run

1. Open the project in **Visual Studio** with MASM support
2. Build the solution
3. Run the executable
4. Enter a number between 0 and 100 when prompted
5. View the computed `shaw(n)` value
6. Choose whether to continue (1 = Yes, 0 = No)

---

