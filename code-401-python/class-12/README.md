# Stacks and Queues

## What Stack and Queue means :
- Stack is a container of objects that are inserted and removed according to the last-in first-out (LIFO) principle.

- Queue is a container of objects that are inserted and removed according to the first-in first-out (FIFO) principle.

## Work principle for Stack :

### In the pushdown stacks only two operations are allowed: 
- push the item into the stack
-  and pop the item out of the stack. 
### A stack is a limited access data structure - elements can be added and removed from the stack only at the top.
###  push adds an item to the top of the stack, pop removes the item from the top.

## Types of stack:
- Last In First Out (LIFO): The last object into a stack is the first object to leave the stack, used by a stack
![LIFO](/code-401-python/class-12/lifo_stack.webp)

- Stack: First In Last Out (FILO): The first object or item in a stack is the last object or item to leave the stack.

## There are some basic operations that allow us to perform different actions on a stack.

- Push: Add an element to the top of a stack
- Pop: Remove an element from the top of a stack.

- IsEmpty: Check if the stack is empty.

- int top(): This operation will return the last inserted element that is at the top without removing it.

- int size(): This operation will return the size of the stack i.e. the total number of elements present in the stack.

- IsFull: Check if the stack is full.

- Peek: Get the value of the top element without removing it.

## Working of Stack Data Structure
The operations work as follows:
![stack_operation](/code-401-python/class-12/stack-operations.webp)

- A pointer called TOP is used to keep track of the top element in the stack.
- When initializing the stack, we set its value to -1 so that we can check if the stack is empty by comparing TOP == -1.
- On pushing an element, we increase the value of TOP and place the new element in the position pointed to by TOP.
- On popping an element, we return the element pointed to by TOP and reduce its value.
- Before pushing, we check if the stack is already full
- Before popping, we check if the stack is already empty

## Application of Stack in real life:

- CD/DVD stand.
- Stack of books in a book shop.
- Undo and Redo mechanism in text editors.
- The history of a web browser is stored in the form of a stack.
- Call logs, E-mails, and Google photos in any gallery are also stored in form of a stack.
- YouTube downloads and Notifications are also shown in LIFO format(the latest appears first ).
- Advantages of Stack:


## Work principle for Queue :

### in queue new additions to a line made to the back of the queue, while removal (or serving) happens in the front.

###  In the queue only two operations are allowed enqueue and dequeue.
-  Enqueue :  means to insert an item into the back of the queue.
-  dequeue : means removing the front item.

## Types of Queue :
- First In First Out (FIFO): The first object into a queue is the first object to leave the queue, used by a queue.

-  Last In Last Out (LILO): The last object or item in a queue is the last object or item to leave the queue.


## Some other applications of Queue:
- Applied as waiting lists for a single shared resource like CPU, Disk, and Printer.
- Applied as buffers on MP3 players and portable CD players.
- Applied on Operating system to handle the interruption.
- Applied to add song at the end or to play from the front.
- Applied on WhatsApp when we send messages to our friends and they don’t have an internet connection then these messages are queued on the server of WhatsApp.
