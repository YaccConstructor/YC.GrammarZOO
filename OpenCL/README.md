# OpenCL C function definitions

A basic grammar for OpenCL C 2.0 function definitions. The purpose of this parser and lexer is to extract
function definitions from OpenCL C code for further usage in F# code; note that this is not a fully-functional
translator for checking and/or translating OpenCL C code.

For the moment the following restrictions apply:

* only function definitions are supported as top-level declarations
* only basic data types are supported (see below in the grammar)
* unions are not supported
* anonymous structs as function parameters are not supported
* `__attribute__` specifiers for kernel functions are not supported
* `inline` function specifier is not supported in OpenCL C
* Unicode in identifiers is not supported
* type casting in function definitions is not supported
