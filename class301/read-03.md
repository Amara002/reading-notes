 # Lists and keys
 
- **What does .map() return?**
    ***We return a '< li >' element for each item.***

- **If I want to loop through an array and display each value in JSX, how do I do that in React?**
    ***we loop an array using  map()*** 

- **Each list item needs a unique** ***key.***

- **What is the purpose of a key?**
    ***key is a special string attribute you need to include when creating lists of elements.***

# The spread Operator

1. **What is the spread operator?**
***The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.***

2. **List 4 things that the spread operator can do.**
   - ***Copying an array.***
   - ***Concatenating or combining arrays.***
   - ***Using Math functions.***
   - ***Using an array as arguments.*** 

3. **Give an example of using the spread operator to combine two arrays.**
- ***const arr1 = [1,2,3]***
- ***const arr2 = [4,5,6]***
- ***const arr3 = [...arr1, ...arr2] //arr3 ==> [1,2,3,4,5,6]***

4. **Give an example of using the spread operator to add a new item to an array.**
- ***let numberStore = [0, 1, 2];***
- ***let newNumber = 12;***
- ***numberStore = [...numberStore, newNumber];***

5. **Give an example of using the spread operator to combine two objects into one**
- ***var a = { name:'test1'}***
- ***var b = {name:'test2'}***
- ***var c = {...a,...b}***
- ***console.log(c)***

# How to pass functions between components


1. **In the video, what is the first step that the developer does to pass functions between components?**
***Create a function where the state is inside the same component.***
2. **In your own words, what does the increment function do?**
***increase the value when we press on the button***
3. **How can you pass a method from a parent component into a child component?**
***we can do that by props.***
4. **How does the child component invoke a method that was passed to it from a parent component?**
***we create a new function inside the child then invoke the function from the parent after we pass it inside the parent.***


