# Decisions

#### Raw Pointer vs Smart Pointers

I chose raw pointer over smart pointers because there is no such "memory leak" in a compiler, especially for the compiler that only runs once: after generating the LLVM bitcode file, the compiler ends its life and LLVM should concern the rest of things. The only thing matters is the generated code but not the compiler itself. We need to think about how to make the generated bitcode more memory-safe rather than think a very short-lived compiler.
