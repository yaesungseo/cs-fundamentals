# Programming Languages
## Core idea
A language specifies how programs are expressed. An implementation determines how they run. Compare languages by their type systems, memory models, ecosystems, and execution environments—not just syntax.

## Useful distinctions
- **Static typing:** many type checks happen before execution, as in Java.
- **Dynamic typing:** types are associated with runtime values and many checks happen during execution, as in Python.
- **Compilation:** translates a program into another representation.
- **Interpretation:** executes a representation through another program.
- **JIT compilation:** compiles code during execution.

Compilation and interpretation are not mutually exclusive. Common Python and Java implementations both use intermediate representations, though their execution strategies differ.

## Languages in context
- **Python:** concise syntax and dynamic typing; widely used for scripts, automation, and data work.
- **Java:** static typing, garbage collection, and a JVM-based ecosystem.
- **C:** explicit memory management and low-level control.
- **C++:** static typing, generic programming, and tools such as RAII for managing resources.
- **JavaScript:** dynamic typing and a central role in browser programming; also runs outside browsers.

These are typical characteristics, not limits on what each language can build. Memory safety and performance depend on both the language and how it is used.

## Example
In Python, a name can refer to an integer and later to a string. A Java variable declared as int cannot later hold a string. Neither choice alone guarantees a correct program.

## Try it
Implement the same input-validation task in Python and Java. Compare error handling and type checks separately from the number of lines.

## Expand next
Scope and lifetime; references and values; garbage collection; programming paradigms; standard libraries; package managers.

## References
[Python tutorial](https://docs.python.org/3/tutorial/) · [Learn Java](https://dev.java/learn/)

[Back to index](../../README.md)
