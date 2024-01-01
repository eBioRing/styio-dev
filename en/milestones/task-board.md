# Task Board

<table><thead><tr><th width="208">Code</th><th>Name</th></tr></thead><tbody><tr><td>I[0-9]+</td><td>Implementation</td></tr><tr><td>DS[0-9]+</td><td>Data Structure</td></tr><tr><td>F[0-9]+</td><td>Feature</td></tr><tr><td>O[0-9]+</td><td>Optimization</td></tr><tr><td>E[0-9]+</td><td>Exception</td></tr><tr><td></td><td></td></tr><tr><td>TSys[0-9]+</td><td>Type System</td></tr><tr><td>TInfer[0-9]+</td><td>Type Inference</td></tr><tr><td>Gen[0-9]+</td><td>LLVM IR Generation</td></tr><tr><td></td><td></td></tr></tbody></table>

## \[E1] Code Text Locate

#### **Done (Method)**

Use global position to locate the line number (binary search).

Add extra line seperation.

Lable the current line with offset (position of curr char - start of this line).

#### Derived Problem

1. How to design and implement exceptions for a compiler?

{% embed url="https://llvm.org/docs/ExceptionHandling.html" %}

## \[E1] Error Message Format



## \[E1] For Parsing (Parser Error)



## \[E1] For Type Checking (Type Error)



## \[TInfer1] Type Check: Integer, Float



## \[TInfer1] Type Convert: Integer -> Float



## \[I1] Arithmetic Calculation

Types:

1. \[ true | false ]
2. i32, i64
3. f32, f64

Operators:

1. Addition ( + )
2. Subtraction ( - )
3. Mutiplication ( \* )
4. Division ( / )
5. Modulo ( % )



## \[I1] Custom Type



## \[I1] Constant Initialization

Types:

1. **Integer**: i32, i64
2. **Float**: f32, f64
3. **Resource Identifier**



## \[DS1] Array (Fixed Length)



## \[DS1] Struct

### Heterogeneous: Any



## \[DS1] List

### Homogeneous

#### Integer

1. i32 (type: int / integer)
2. i64

#### Float / Double

1. f32 (type: float)
2. f64 (type: double)

### Heterogeneous: Any



## \[DS1] String

```
struct {
  ptr,
  len,
  capacity
}
```



## \[F1] URLs Are Not Strings

We need a feasible way to create, modify and operates URLs.

{% embed url="https://news.ycombinator.com/item?id=21765788" %}

## \[O1] Parse URLs

