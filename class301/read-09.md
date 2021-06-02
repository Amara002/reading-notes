# Functional Programming Concepts


1. **What is functional programming?**
***Functional programming (often abbreviated FP) is the process of building software by composing pure functions, avoiding shared state, mutable data, and side-effects. Functional programming is declarative rather than imperative, and application state flows through pure functions. Contrast with object oriented programming, where application state is usually shared and colocated with methods in objects.***

2. **What is a pure function and how do we know if something is a pure function?**
***It returns the same result if given the same arguments***

3. **What are the benefits of a pure function?**
***The code’s definitely easier to test. We don’t need to mock anything.***

4. **What is immutability?**
***When data is immutable, its state cannot change after it’s created. If you want to change an immutable object***

5. **What is Referential transparency?**
***A function that consistently yields the same result for the same input, is referentially transparent.***


# Modules

1. **What is a module?**
***Module in Node. js is a simple or complex functionality organized in single or multiple JavaScript files which can be reused throughout the Node. js application. Each module in Node. js has its own context, so it cannot interfere with other modules or pollute global scope.***

2. **What does the word ‘require’ do?**
***The builtin require function is the easiest way to include modules that exist in separate files. The basic functionality of require is that it reads a JavaScript file, executes the file, and then proceeds to return the exports object.***

3. **How do we bring another module into the file the we are working in?**
***By using require ***

4. **What do we have to do to make a module available?**
***export the module and specify what I want to export.***