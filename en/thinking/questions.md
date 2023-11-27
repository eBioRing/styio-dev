# Questions

## How many components does Styio have?

#### Compiler - Compilation (<mark style="color:purple;">Progressing</mark>)

* Parser (<mark style="color:purple;">progressing</mark>)
* Type Checking (<mark style="color:purple;">framework established</mark>)
* LLVM IR Code Generation (<mark style="color:purple;">framework established</mark>)
* Abstract I/O Model (<mark style="color:purple;">awaiting decision</mark>)

#### Compiler - Runtime (<mark style="color:purple;">Progressing</mark>)

* Memory Allocator (<mark style="color:purple;">awaiting decision</mark>)
* Garbage Collector (GC) (<mark style="color:purple;">awaiting decision</mark>)
* eBPF Traffic Tracing Optimizer (<mark style="color:purple;">awaiting decision</mark>)

#### I/O Model

* io\_uring: network & file
* coroutine | async / await (<mark style="color:purple;">awaiting decision</mark>)

#### Toolchain - Code Linter (<mark style="color:red;">Pending</mark>)

Prerequisites: Visual Studio Code + Node.js

#### Toolchain - Debugger (<mark style="color:red;">Pending</mark>)

#### Toolchain - Package Manager (<mark style="color:red;">Pending</mark>)

***

Labels:

1. <mark style="color:red;">Pending</mark>: Requirement Analysis & Feasibility Study
2. <mark style="color:purple;">Designing / Evolving / Deciding</mark>: Framework Establishment & Final Decision
3. <mark style="color:green;">Progressing</mark>: Functionality Implementation&#x20;
4. <mark style="color:yellow;">Testing</mark>
5. <mark style="color:blue;">Done</mark>

***

After Done:

1. Stage I : A Basic Prototype
2. Stage II : Review
3. Stage III : Formalize & Verify
4. Stage IV : Complete -> Clean & Refactor
5. Stage V : Prepare for Extensions

## Milestones

Programming Language

* Syntax Design (Stage I) - <mark style="color:blue;">Done</mark>
* Parser (Stage I) - <mark style="color:blue;">Done</mark>
* Type Hinting & Checking (Stage I) - <mark style="color:purple;">Designing</mark>
* LLVM Code Generator (Stage I) - <mark style="color:green;">Progressing</mark>
* Code Linter (Stage I) - <mark style="color:red;">Pending</mark>

I/O Model

* io\_uring: high-level abstraction (Stage I) - <mark style="color:red;">Pending</mark>
* Memory Allocator (Stage I)
* Garbage Collector (Stage II)

Review

* Syntax Design (Stage II)
* Parser (Stage II)
* Type Hinting & Checking (Stage II)
* LLVM Code Generator (Stage II)
* Documentation

Optimization

* eBPF Traffic Tracing Optimizer (Stage I)

Toolchain

* Debugger (Stage I)

## What if we have funding?

