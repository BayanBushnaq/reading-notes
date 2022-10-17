# Linkedlist and Data structures 
## What is the data structure ?
###  data structure is a specialized format for organizing, processing, retrieving and storing data. There are several basic and advanced types of data structures, all designed to arrange data to suit a specific purpose. Data structures make it easy for users to access and work with the data they need in appropriate ways. 

## Why data structers important ?
### Data Structures are necessary for designing efficient algorithms. It provides reusability and abstraction. Using appropriate data structures can help programmers save a good amount of time while performing operations such as storage, retrieval, or processing of data. Manipulation of large amounts of data is easier.

## How are data structures used?
### data structures are used to implement the physical forms of abstract data types. Data structures are a crucial part of designing efficient software.

## Usages of data structures :
- Storing data Managing resources and services. 
- Data exchange. 
- Ordering and sorting. 
- Indexing. Searching. 
- Scalability.  

## Data structures are often classified by their characteristics.  
 1- Linear or non-linear.
 2- Homogeneous or heterogeneous.
 3- Static or dynamic.

 ### Types of data structures
## The data structure type used in a particular situation is determined by the type of operations that will be required or the kinds of algorithms that will be applied.
- Array.
- Stack. 
- Linked list.
- Tree.
- Heap.
- Graph.
- Trie. 
- Hash table.

	![classification of data structures](/code-401-python/class-09/Classification.jpg)

### How to choose a data structure
## When choosing a data structure for a program or application, developers should consider the answers to the following three questions:

- Supported operations. What functions and operations does the program need?
- Computational complexity. What level of computational performance is tolerable? For speed, a data structure whose operations execute in time linear to the number of items managed -- using Big O Notation: O(n) -- will be faster than a data structure whose operations execute in time proportional to the square of the number of items managed -- O(n^2).
- Programming elegance. Are the organization of the data structure and its functional interface easy to use?

### Here is some advices when you want to determine which data structre is suitable for your problem:
- Linked lists: are best if a program is managing a collection of items that don't need to be ordered, constant time is required for adding or removing an item from the collection and increased search time is OK.
-  Stacks: are best if the program is managing a collection that needs to support a LIFO order.
- Queues :  should be used if the program is managing a collection that needs to support a FIFO order.
- Binary trees: are good for managing a collection of items with a parent-child relationship, such as a family tree.
- Binary search trees: are appropriate for managing a sorted collection where the goal is to optimize the time it takes to find specific items in the collection.
- Graphs :work best if the application will analyze connectivity and relationships among a collection of individuals in a social media network.


### What is LinkedList ?
## Linked Lists are a data structure that store data in the form of a chain. The structure of a linked list is such that each piece of data has a connection to the next one (and sometimes the previous data as well). Each element in a linked list is called a node.

### Advantages of Linked Lists:
- Because of the chain-like system of linked lists, you can add and remove elements quickly. 
- Linear data structures are often easier to implement using linked lists.
- Linked lists also don't require a fixed size or initial size due to their chainlike structure.

### Disadvantages of a Linked Lists:
- More memory is required when compared to an array. This is because you need a pointer (which takes up its own memory) to point you to the next element.
- Search operations on a linked list are very slow. Unlike an array, you don't have the option of random access.

### When Should You Use a Linked List?
- if You don't know how many items will be in the list
- if You don't need random access to any elements
- if You want to be able to insert items in the middle of the list.
- if You need constant time insertion/deletion from the list