 LEX-Project – Lexical Analyzer for C-Minus

This project is a simple **Lexical Analyzer (Scanner)** for the C-Minus programming language.  
It was developed in C language as part of a compiler course.

 🔍 What does it do?

The Lexical Analyzer reads C-Minus source code (e.g. `.cm` files) and breaks it down into **tokens**.  
Tokens are things like:

- Keywords (`if`, `while`, `int`, etc.)
- Identifiers (variable names)
- Numbers
- Operators (`+`, `-`, `=`, etc.)
- Symbols (`;`, `(`, `)`, etc.)

 ⚙️ How it works

The scanner uses a **state machine** implemented in C to:

1. Read the source code character by character.
2. Ignore whitespaces and comments.
3. Recognize tokens based on DFA (Deterministic Finite Automaton).
4. Print the recognized tokens with their type and line number.

 📁 Main Files

- `scan.c`: Contains the main logic of the lexical analyzer (state machine).
- `main.c`: Runs the program and calls the scanner.
- `arithmetic.cm`, `nested_if.cm`: Test input files.

 ✅ Output Example

For an input like:

```c
if (a == 5) write a;
