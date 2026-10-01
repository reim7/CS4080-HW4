# CS4080 HW4 — Chapters 8 & 9 Challenges

This repository contains my Java implementation work for the Chapter 8 and Chapter 9 challenges from *Crafting Interpreters*.

## Implemented coding challenges

- Chapter 8, Challenge 1: REPL supports both statements and bare expressions.
- Chapter 8, Challenge 2: Reading a declared but uninitialized variable produces a runtime error.
- Chapter 9, Challenge 3: Added `break;` support. `break` is only valid inside loops and exits the nearest enclosing loop.

## Source structure

- `com/craftinginterpreters/lox/` — jlox scanner, parser, AST, environment, and interpreter.
- `com/craftinginterpreters/tool/GenerateAst.java` — AST generator updated to support the empty-field `Break` statement.

## Compile

```bash
javac com/craftinginterpreters/lox/*.java
```

## Run

```bash
java com.craftinginterpreters.lox.Lox
```
