# Language Basics

## Variables
***The Java programming language defines the following kinds of variables:***
- ***Instance Variables (Non-Static Fields) Technically speaking, objects store their individual states in "non-static fields"***
- ***Class Variables (Static Fields) A class variable is any field declared with the static modifier***
- ***Local Variables Similar to how an object stores its state in fields, a method will often store its temporary state in local variables.***
- ***Parameters:The important thing to remember is that parameters are always classified as "variables" not "fields". This applies to other parameter-accepting constructs as well (such as constructors and exception handlers)***
- ***Naming:If the name you choose consists of only one word, spell that word in all lowercase letters. If it consists of more than one word, capitalize the first letter of each subsequent word. The names gearRatio and currentGear are prime examples of this convention. If your variable stores a constant value, such as static final int NUM_GEARS = 6, the convention changes slightly, capitalizing every letter and separating subsequent words with the underscore character. By convention, the underscore character is never used elsewhere.***

## Operators
![Operators](class401/OperatorJava.PNG)


## Expressions, Statements, and Blocks
- ***Expressions:An expression is a construct made up of variables, operators, and method invocations, which are constructed according to the syntax of the language, that evaluates to a single value.***
- ***Statements:Statements are roughly equivalent to sentences in natural languages. A statement forms a complete unit of execution. The following types of expressions can be made into a statement by terminating the expression with a semicolon (;)***
- ***Blocks:A block is a group of zero or more statements between balanced braces and can be used anywhere a single statement is allowed.***

## Control Flow Statements
***The statements inside your source files are generally executed from top to bottom, in the order that they appear. Control flow statements, however, break up the flow of execution by employing decision making, looping, and branching, enabling your program to conditionally execute particular blocks of code. This section describes the decision-making statements (if-then, if-then-else, switch), the looping statements (for, while, do-while), and the branching statements (break, continue, return) supported by the Java programming language.***

# What does it mean to compile code?
***When you compile code, the compilor (usually another program) takes the program the human wrote, and converts it into the program the computer can understand (i.e. converts from Java to machine language). The very short version could be, yes, compile means to make the code executable. Something you may run into is people saying code does or does not compile. This means the compilor they used checks to make sure their program is written correctly according to the rules of the programming language. For example, most programming languages make you put a semicolon (;) at the end of every line. A very common mistake is to forget that semicolon, so when you try and compile the compilor gives you an error.***

# Making Sense of Java’s API Documentation
***Java has a whole collection of grammatical features, but Java is much more than just a big set of grammar rules. Java has a standard Application Programming Interface —a huge library consisting of over 4,000 classes, each with its own functionality, its own limitations, and its own rules for effective use.***