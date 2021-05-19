# class 10

## What is a Stack
A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.

#### stack's terminology 
1. Push - Nodes or items that are put into the stack are pushed
1. Pop - Nodes or items that are removed from the stack are popped. 
1. Top - This is the top of the stack
1. Peek - When you peek you will view the value of the top Node in the stack.
1. IsEmpty - returns true when stack is empty otherwise returns false.

***Stacks follow these concepts:*** 
- FILO: First In Last Out
- LIFO: Last In First Out

#### Stack Visualization
![stack](./images/stack1.png)

***Pushing, Popping, Peeking and IsEmpty  a Node onto a stack will always be an `O(1)` operation.***

## What is a Queue

1. Enqueue - Nodes or items that are added to the queue.
1. Dequeue - Nodes or items that are removed from the queue.
1. Front - This is the front/first Node of the queue.
1. Rear - This is the rear/last Node of the queue.
1. Peek - When you peek you will view the value of the front Node in the queue.
1. IsEmpty - returns true when queue is empty otherwise returns false.

***Queues follow these concepts:***
- FIFO: First In First Out
- LILO: Last In Last Out

#### Queue Visualization
![Queue](./images/Queue.png)

***All Queue operations are `O(1)` operations***