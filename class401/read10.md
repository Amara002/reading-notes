# Stacks and Queues

## What is a Stack
***A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.***

***Common terminology for a stack is***

1. ***Push - Nodes or items that are put into the stack are pushed***
2. ***Pop - Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised.***
3. ***Top - This is the top of the stack.***
4. ***Peek - When you peek you will view the value of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised.***
5. ***IsEmpty - returns true when stack is empty otherwise returns false.***

## FILO

***First In Last Out***
***This means that the first item added in the stack will be the last item popped out of the stack.***

## Stack Visualization

### Push O(1)
***Pushing a Node onto a stack will always be an O(1) operation. This is because it takes the same amount of time no matter how many Nodes (n) you have in the stack.***

### Pop O(1)
***Popping a Node off a stack is the action of removing a Node from the top. When conducting a pop, the top Node will be re-assigned to the Node that lives below and the top Node is returned to the user.***

### Peek O(1)
***When conducting a peek, you will only be inspecting the top Node of the stack.***

### IsEmpty O(1)
***Here is the pseudocode for isEmpty***

## Queue Visualization

### Enqueue O(1)
***When you add an item to a queue, you use the enqueue action. This is done with an O(1) operation in time because it does not matter how many other items live in the queue (n); it takes the same amount of time to perform the operation.***

### Dequeue O(1)
***When you remove an item from a queue, you use the dequeue action. This is done with an O(1) operation in time because it doesn’t matter how many other items are in the queue, you are always just removing the front Node of the queue.***

### Peek O(1)
***When conducting a peek, you will only be inspecting the front Node of the queue.***

### IsEmpty O(1)
***Here is the pseudocode for isEmpty***
