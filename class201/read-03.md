# Lists
***HTML provides us with three different types of list which is as follows:***
- **'< ol >': Ordered lists are lists where each item in the list is numbered.**
- **'< ul >': Unordered lists are lists that begin with a bullet point.**
   > Each item in the list is placed between an opening '< li >' tag and a closing '< /li >' tag.And it is used inside ordered and unordered lists.
- **Definition lists are made up of a set of terms along with the definitions for each of those terms.The definition list is created with the '< dl >' element and usually consists of a series of terms and their definitions.Inside the '< dl >' element you will usually see pairs of '< dt >' and '< dd >' elements.**

  > ***Note: Lists can be nested inside one another***

# Boxes
***CSS treats each HTML element as if it has its own box.*** 

## Box dimensions
***You can use CSS to control the dimensions of a box though:***
- **width, height**
- **min-width, max-width("Some page designs expand and shrink to fit the size of the user's screen.")**
- **min-height, max-height("In the same way that you might want to limit the width of a box on a page.")**

## Overflowing contents
***The overflow property tells the browser what to do if the content contained within a box is larger than the box itself. It can have one of two values as:***
- **Hidden: This property simply hides any extra content that does not fit in the box.**
- **scroll: This property adds a scrollbar to the box so that users can scroll to see the missing content.**

## Border, Margin & Padding
***You can also control the borders, margin and padding for each box with CSS.***
- **Border: Every box has a border (even if it is not visible or is specified to be 0 pixels wide). The border separates the edge of one box from another**
- **Margin: Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes.**
- **Padding: is the space between the border of a box and any content contained within it.**

### Important noted 

- **It is possible to hide elements using the display and visibility properties.**
- **Block-level boxes can be made into inline boxes, and inline boxes made into block-level boxes.**

## USING IF ... ELSE STATEMENTS
***Here you can see that an if ... e 1 se statement allows you to provide two sets of code:*** 
1. **one set if the condition evaluates to true** 
2. **another set if the condition is false** 

## Logical operators
***Logical operators allow you to compare the results of more than one Comparison operator.***

**We have three main logical operator as:**
1. &&(logical and) this operator tests more than one condition.
2. || (logical or) this operator tests at least one condition.
3. ! (not operator) this operator take a single boolean value and inverts it.

## loops
***Loops check a condition. if it returns true, a code block will run. Then the condition will be checked again and if it still returns true, the code block will run again. it repeats until the condition returns false.***
***There are three main types of loops which is as follows:***
1. **For : if you need to run code a specific number of times.This loop made up of three statements(initialization(i=0),condition(i<10),update(i++))**
2. **While : if you do not know how many times the code should run and the code will continue to loop for as long as the condition is true.**
3. **Do while : is very similar to the while loop,but it will always run the statements inside the curly braces at least once,even if the condition evaluates to false.**