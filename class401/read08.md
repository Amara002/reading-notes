## SOLID stands for:

- ***S - Single-responsiblity Principle***
- ***O - Open-closed Principle***
- ***L - Liskov Substitution Principle***
- ***I - Interface Segregation Principle***
- ***D - Dependency Inversion Principle***

## SOLID: The First 5 Principles of Object Oriented Design
1. ***Single-Responsibility Principle***

> ***Single-responsibility Principle (SRP) states:  A class should have one and only one reason to change, meaning that a class should have only one job.***

2. ***Open-Closed Principle***

> ***Open-closed Principle (OCP) states: Objects or entities should be open for extension but closed for modification.***

3. ***Liskov Substitution Principle***

> ***Liskov Substitution Principle states: Let q(x) be a property provable about objects of x of type T. Then q(y) should be provable for objects y of type S where S is a subtype of T.***

4. ***Interface Segregation Principle***

> ***Interface segregation principle states: A client should never be forced to implement an interface that it doesn’t use, or clients shouldn’t be forced to depend on methods they do not use.***

5. ***Dependency Inversion Principle***

> ***Dependency inversion principle states: Entities must depend on abstractions, not on concretions. It states that the high-level module must not depend on the low-level module, but they should depend on abstractions.***

## The SOLID Principles in Real Life

- ***s is for single responsibility principle: the single responsibility principle (srp) asserts that a class or module should do one thing only. now, this is kind of subjective, so the principle is reinforced with the heuristic that the class or module should have only one reason to change.***

- ***o is for open/closed principle: the open/closed principle states that code entities should be open for extension, but closed for modification. to put this more concretely, you should write a class that does what it needs to flawlessly and not assuming that people should come in and change it later. it's closed for modification, but it can be extended by, for instance, inheriting from it and overriding or extending certain behaviors. an example of running afoul of the open-closed principle would be to have a switch statement somewhere that you needed to go in and add to every time you wanted to add a menu option to your application.***

- ***l is for liskov substitution principle: the liskov substitution principle (lsp) is the one here that is most unique to object-oriented programming. the lsp says, basically, that any child type of a parent type should be able to stand in for that parent without things blowing up.***

- ***i is for interface segregation principle: the interface segregation principle (isp) says that you should favor many, smaller, client-specific interfaces over one larger, more monolithic interface. in short, you don't want to force clients to depend on things they don't actually need. imagine your code consuming some big, fat interface and having to re-compile/deploy with annoying frequency because some method you don't even care about got a new signature.***

- ***d is for dependency inversion: the dependency inversion principle (dip) encourages you to write code that depends upon abstractions rather than upon concrete details. you can recognize this in the code you read by looking for a class or method that takes something generic like "stream" and performs operations on it, as opposed to instantiating a specific filestream or stringstream or whatever. this gives the code in question a lot more flexibility -- you can swap in anything that conforms to the stream abstraction and it will still work.*** 


