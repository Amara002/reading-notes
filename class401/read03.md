# Java Primitives versus Objects
- ***Java has a two-fold type system consisting of primitives such as int, boolean and reference types such as Integer, Boolean. Every primitive type corresponds to a reference type.***

- ***Every object contains a single value of the corresponding primitive type. The wrapper classes are immutable (so that their state can't change once the object is constructed) and are final (so that we can't inherit from them).***

- ***The decision what object is to be used is based on what application performance we try to achieve, how much available memory we have, the amount of available memory and what default values we should handle.***

# Exception
***An exception is an event, which occurs during the execution of a program, that disrupts the normal flow of the program's instructions.***

# The Catch or Specify Requirement
***Valid Java programming language code must honor the Catch or Specify Requirement. This means that code that might throw certain exceptions must be enclosed by either of the following:***

   1. ***A try statement that catches the exception. The try must provide a handler for the exception, as described in Catching and Handling Exceptions.***
   2. ***A method that specifies that it can throw the exception. The method must provide a throws clause that lists the exception, as described in Specifying the Exceptions Thrown by a Method.***

> ***NOTE:Code that fails to honor the Catch or Specify Requirement will not compile.***
### The Three Kinds of Exceptions
1. ***checked exception: These are exceptional conditions that a well-written application should anticipate and recover from.***
2. ***the error: These are exceptional conditions that are external to the application, and that the application usually cannot anticipate or recover from.***

3. ***the runtime exception. These are exceptional conditions that are internal to the application, and that the application usually cannot anticipate or recover from.***

# Catching and Handling Exceptions
***This section describes how to use the three exception handler components — the try, catch, and finally blocks — to write an exception handler. Then, the try-with-resources statement, introduced in Java SE 7, is explained. The try-with-resources statement is particularly suited to situations that use Closeable resources, such as streams.***

# Scanning
***Objects of type Scanner are useful for breaking down formatted input into tokens and translating individual tokens according to their data type.***