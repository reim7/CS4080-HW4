
CS 4080 - Homework 4

This repository contains the programming portions of Homework 4 

Chapter 8 - Statements and State

REPL

I modified the Lox REPL to support both statements and expressions. Statements execute normally, while expressions are evaluated and their results are displayed automatically without requiring a print statement.

Files: Parser.java, Interpreter.java, Lox.java

Uninitialized Variables

I modified the interpreter so that accessing a variable before it has been initialized or assigned produces a runtime error instead of automatically returning nil.

Files: Interpreter.java, test_uninitialized.lox

Chapter 9 - Control Flow

Break Statement

I added support for the break; statement in Lox. The parser checks whether break is used inside a loop and reports an error if it is not. When executed, break exits the nearest enclosing loop, including when it appears inside nested blocks or if statements.

Files: Scanner.java, Parser.java, Interpreter.java, TokenType.java, Stmt.java, GenerateAst.java

Testing

I included test files to demonstrate the changes made to the interpreter.

test_break.lox — Tests the break statement inside a loop.

test_uninitialized.lox — Tests the runtime error when accessing an uninitialized variable.

Written Responses

The written responses for the Chapter 8 and Chapter 9 challenges are included in my submitted Homework 4 PDF.
