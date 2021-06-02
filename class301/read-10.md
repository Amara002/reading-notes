# In memory storage


1. **What is a ‘call’?**
***The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.***

2. **How many ‘calls’ can happen at once?**
**only one call**

3. **What does LIFO mean?**
***last in first out***

5. **What causes a Stack Overflow?**
***A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.***

# Error massages

1. **What is a ‘refrence error’?**
***The ReferenceError object represents an error when a non-existent variable is referenced.***

2. **What is a ‘syntax error’?**
***The SyntaxError object represents an error when trying to interpret syntactically invalid code. It is thrown when the JavaScript engine encounters tokens or token order that does not conform to the syntax of the language when parsing code.***

3. **What is a ‘range error’?**
***It means that somewhere in your code, you are calling a function which in turn calls another function and so forth, until you hit the call stack limit. This is almost always because of a recursive function with a base case that isn't being met***

4. **What is a ‘tyep error’?**
***The TypeError object represents an error when an operation could not be performed, typically (but not exclusively) when a value is not of the expected type. A TypeError may be thrown when: an operand or argument passed to a function is incompatible with the type expected by that operator or function.***

5. **What is a breakpoint?**
***At each breakpoint, JavaScript will stop executing, and let you examine JavaScript values. After examining values, you can resume the execution of code (typically with a play button).***

6. **What does the word ‘debugger’ do in your code?**
***The breakpoint can also be achieved by putting a debugger statement in your code in the line you want to break.***

