# Compiler Design Lab

A collection of **Compiler Design laboratory programs** implemented using **C, Flex (Lex), and Bison (Yacc)**. This repository demonstrates the fundamental phases of a compiler, including lexical analysis, syntax analysis, parsing techniques, and simple compiler construction experiments.

---

## 📚 Course Information

- **Course:** Compiler Design
- **Language:** C
- **Tools:** Flex, Bison, GCC
- **Platform:** Linux / Ubuntu (Recommended)

---

# Repository Structure

```text
Compiler-Design/
│
├── Lab-1/
├── Lab-2/
├── Lab-3/
├── Lab-4/
├── Lab-5/
├── Lab-6/
├── Lab-7/
├── Lab-8/
├── README.md
└── LICENSE
```

Each lab contains:

```text
Lab-x/
│
├── source files
├── input files
├── output screenshots (optional)
├── README.md (optional)
```

---

# Prerequisites

Install the required packages before running the programs.

## Ubuntu / Debian

```bash
sudo apt update
sudo apt install flex bison gcc make
```

Verify installation:

```bash
flex --version
bison --version
gcc --version
```

---

# Topics Covered

- Introduction to Compiler Design
- Lexical Analysis
- Syntax Analysis
- Regular Expressions
- Context-Free Grammar (CFG)
- Parse Trees
- LL Parsing
- LR Parsing
- Shift Reduce Parsing
- Operator Precedence Parsing
- Recursive Descent Parser
- Flex Programming
- Bison Programming
- Error Detection
- Error Recovery
- Symbol Table
- Intermediate Code Generation
- Syntax Directed Translation

---

# Labs

## Lab 1

- Introduction to Flex
- Token Recognition

## Lab 2

- Lexical Analyzer using Flex

Features:

- Keywords
- Identifiers
- Operators
- Constants
- Delimiters

---

## Lab 3

- Lexical Analyzer for C Programs

Recognizes:

- Keywords
- Variables
- Numbers
- Comments
- Operators

---

## Lab 4

- Expression Parser using Bison

Supports:

- Arithmetic Expressions
- Parentheses
- Operator Precedence

---

## Lab 5

### Syntax Analyzer for IF-ELSE Statements

Features:

- Simple if statement
- if-else statement
- Nested if-else
- Dangling else resolution
- Syntax error detection

Example:

```c
if(a>b)
    x=y;

if(a>b)
    x=y;
else
    x=z;

if(a>b)
    if(c>d)
        x=y;
    else
        x=z;
```

---

## Lab 6

- Symbol Table Implementation

Operations:

- Insert
- Search
- Delete
- Display

---

## Lab 7

- Recursive Descent Parser

Supports:

- Arithmetic Grammar
- Recursive Parsing

---

## Lab 8

- Intermediate Code Generation

Generates:

- Three Address Code
- Quadruples
- Triples

---

# Build Instructions

For Flex/Bison programs

Generate parser:

```bash
bison -d filename.y
```

Generate lexical analyzer:

```bash
flex filename.l
```

Compile:

```bash
gcc filename.tab.c lex.yy.c -lfl -o output
```

Run:

```bash
./output
```

---

# Sample Execution

Input

```text
if(a>b) x=y;
```

Output

```text
Valid Statement
```

Input

```text
if(a>b x=y;
```

Output

```text
Syntax Error
```

---

# Learning Outcomes

After completing these labs, you will be able to:

- Understand compiler phases.
- Design lexical analyzers using Flex.
- Develop syntax analyzers using Bison.
- Construct Context-Free Grammars.
- Handle parsing conflicts.
- Resolve the dangling-else problem.
- Generate parse trees.
- Detect and recover from syntax errors.
- Build basic compiler components.

---

# Compiler Phases

```text
Source Program
      │
      ▼
Lexical Analysis
      │
      ▼
Syntax Analysis
      │
      ▼
Semantic Analysis
      │
      ▼
Intermediate Code Generation
      │
      ▼
Code Optimization
      │
      ▼
Target Code Generation
```

---

# References

- Alfred V. Aho, Monica S. Lam, Ravi Sethi, Jeffrey D. Ullman — *Compilers: Principles, Techniques, and Tools (Dragon Book)*
- Flex Documentation
- GNU Bison Documentation

---

# Author

**Manish Sah**

Computer Engineering Student

---

# License

This repository is intended for **educational and learning purposes**.
Feel free to use, modify, and share the code with proper attribution.

---

⭐ If you find this repository useful, consider giving it a star.
