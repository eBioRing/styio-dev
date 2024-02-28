# Add A New AST

It is very complicated and I would suggest avoid doing this, but if it is necessary, here are things we need to do:

#### ASTDecl.hpp

ASTDecl.hpp is the header file for **AST Forward Declaration**. Every AST class need to be declared in this file before adding to any other file.

#### AST.hpp

AST.hpp is the header file that defines all AST classes. Every AST class need to be defined in this file after declared in ASTDecl.hpp.

You must inplement `hint()` function for the new AST class.

### Visitors

Styio has many visitors for double dispatching, and that is in dark.

#### StyioVisitors/ASTAnalyzer.hpp

StyioAnalyzerVisitor is a type derived from AnalyzerVisitor, which is used to convert ast to string and type inference (etc. type checking).&#x20;

1. We need to add the new AST into StyioAnalyzerVisitor type.

```cpp
using StyioAnalyzerVisitor = AnalyzerVisitor< NewAST >
```

2. Add `toString` and `typeInfer` functions into the StyioAnalyzer class.

#### StyioVisitors/ToStringImpl.cpp

Styio uses CRTP to generate virtual functions for each AST. The virtual functions are in the template class `StyioNode`. All virtual functions should be implemented in different files.

ToStringImpl.cpp is the file for `toString` function. We need to implement the `toString` function for the new AST.&#x20;

#### StyioVisitors/TypeInferImpl.cpp

TypeInferImpl.cpp is the file for `typeInfer` function. We need to implement the `typeInfer` function for the new AST.

#### StyioVisitors/CodeGenVisitor.hpp

This is another visitor just like StyioAnalyzerVisitor. It is used to generate LLVM IR.&#x20;

1. We need to add the new AST into StyioCodeGenVisitor type.

```cpp
using StyioCodeGenVisitor = CodeGenVisitor< NewAST >
```

2. Add `getLLVMType` and `toLLVMIR` functions into `StyioToLLVMIR` class.

#### StyioVisitors/CodeGenImpl.cpp

CodeGenImpl.cpp is the file for `toLLVMIR` function. We need to implement the `toLLVMIR` function for the new AST.

#### StyioVisitors/GetTypeImpl.cpp

GetTypeImpl.cpp is the file for `getLLVMType` function. We need to implement the `getLLVMType` function for the new AST.
