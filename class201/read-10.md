# Error Handling and Debugging
***When you are writing JavaScript, do not expect to write it perfectly the first time. Programming is like problem solving: you are given a puzzle and not only do you have to solve it, but you also need to create the instructions that allow the computer to solve it. too.***

## ORDER OF EXECUTION 
***To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run***

## EXECUT.ION CONTEXTS
***The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new  execution context.***

## The Stack
***The javascript interpter processes one line of code at a time.When a statment needs data from another function, it stacks the new function on of the current task***

## UNDERSTANDING SCOPE
***In the interpreter, each execution context has its own va ri ables object. It holds the variables, functions, and parameters available within it. Each execution context can also access its parent's v a ri ables object.***

## UNDERSTANDING ERRORS
***If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handl ing code.***

## ERROR OBJECTS
***Error objects can help you find where your mistakes are and browsers have tools to help you read them.***

## HOW TO DEAL WITH ERRORS
1. ***DEBUG THE SCRIPT TO FIX ERRORS.***
2. ***HANDLE ERRORS GRACEFULLY.***

## A DEBUGGING WORKFLOW
***Debugging is about deduction: eliminating potential causes of an error.***

## BROWSER DEV TOOLS & JAVASCRIPT CONSOLE
***The JavaScript console will tell you when there is a problem with a script, where to look for the problem, and what kind of issue it seems to be.***

## WRITING FROM THE SCRIPT TO THE CONSOLE
***Browsers that have a console have a console object, which has several methods that your script can use to display data in the console. The object is documented in the Console API.***

## WRITING TABULAR DATA
***In browsers that support it, the console. table () method lets you output a table showing:*** 
- ***objects*** 
- ***arrays that contain other objects or arrays***

## WRITING ON A CONDITION
***Using the console. assert() method, you can test if a condition is met, and write to the console only if the expression evaluates to false.***

## BREAKPOINTS
***You can pause the execution of a script on any line using breakpoints. Then you can check the values stored in variables at that point in time.***

## STEPPING THROUGH CODE 
***If you set multiple breakpoints, you can step through them one-by-one to see where values change and a problem might occur.***

## CONDITIONAL BREAKPOINTS
***You can indicate that a breakpoint should be triggered only if a condition that you specify is met. The condition can use existing variables.***

## HANDLING EXCEPTIONS
***If you know your code might fail, use try, catch, and finally. Each one is given its own code block.***

## THROWING ERRORS
***If you know something might cause a problem for your script, you can generate your own errors before the interpreter creates them.***

## THROW ERROR FOR NaN
***If you try to use a string in a mathematical operation (other than in addition), you do not get an error, you get a special value called NaN (not a number).***

> ***Note:The console helps narrow down the area in which the error is located, so you can try to find the exact error.*** 