# Forms

1. **What is a ‘Controlled Component’?**
***A Controlled Component is one that takes its current value through props and notifies changes through callbacks like onChange . A parent component "controls" it by handling the callback and managing its own state and passing the new values as props to the controlled component.***

2. **Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.**
***we should update the state with their responses as soon as they enter them because if we did not update it anything should not change on their responses***  

3. **How do we target what the user is entering if we have an event handler on an input field?**
***by definde a state that works into submit function and call this function inside the form tag***


# The Conditional (Ternary) Operator Explained

1. **Why would we use a ternary operator?**
***Using a conditional, like an if statement, allows us to specify that a certain block of code should be executed if a certain condition is met.***

2. **Rewrite the following statement using a ternary statement:** 
***let math= ((x===y) ? 'true' : 'false';)***