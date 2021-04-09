# Java Primitives vs Objects

## autoboxing and unboxing: 
The process of converting a primitive type to a reference one is called autoboxing, the opposite process is called unboxing.
The decision of what object is to be used is based on what application performance we try to achieve, how much available memory we have, the amount of available memory, and what default values we should handle.

primitive type variables have the following impact on the memory:
- boolean – 1 bit
- int, float – 32 bits

reference type :
- Boolean – 128 bits
- Integer, Float – 128 bits


# Performance:
The performance of a Java code is quite a subtle issue, it depends very much on the hardware on which the code runs, on the compiler that might perform certain optimizations, on the state of the virtual machine, on the activity of other processes in the operating system.


# Default Values:
Default values of the primitive types are 0 (in the corresponding representation, i.e. 0, 0.0d etc) for numeric types, false for the boolean type, \u0000 for the char type. For the wrapper classes, the default value is null.


# What Is an Exception?
An exception is an event, which occurs during the execution of a program, that disrupts the normal flow of the program's instructions.

# The Catch or Specify Requirement:
- try 
- throws 


# Catching and Handling Exceptions:
- The try Block

The first step in constructing an exception handler is to enclose the code that might throw an exception within a try block. In general, a try block looks like the following:
``` 
try {
    code
}
catch and finally blocks . . .
 ```

- The catch Blocks

You associate exception handlers with a try block by providing one or more catch blocks directly after the try block. No code can be between the end of the try block and the beginning of the first catch block.
```
try {

} catch (ExceptionType name) {

} catch (ExceptionType name) {

}
```


- The finally Block
The finally block always executes when the try block exits. This ensures that the finally block is executed even if an unexpected exception occurs. But finally is useful for more than just exception handling — it allows the programmer to avoid having cleanup code accidentally bypassed by a return, continue, or break. Putting cleanup code in a finally block is always a good practice, even when no exceptions are anticipated.


# Scanning:
## Objects of type Scanner are useful for breaking down formatted input into tokens and translating individual tokens according to their data type. By default, a scanner uses white space to separate tokens. (White space characters include blanks, tabs, and line terminators. For the full list, refer to the documentation for Character.isWhitespace.) 


