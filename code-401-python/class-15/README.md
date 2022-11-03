# Tree Data Structure

## what is Tree data structure ? 
### A tree is a nonlinear hierarchical data structure that consists of nodes connected by edges.

## Why Tree Data Structure?
### Other data structures such as arrays, linked list, stack, and queue are linear data structures that store data sequentially. In order to perform any operation in a linear data structure, the time complexity increases with the increase in the data size. But, it is not acceptable in today's computational world.

## Tree Terminologies:

- Node :
  - A node is an entity that contains a key or value and pointers to its child nodes.

- Edge :
  - the link between any two nodes.

- Root :
  - the topmost node of a tree.

- Height of a Node :
  -  the longest path from the node to a leaf node.

- Depth of a Node :
  - the number of edges from the root to the node.

- Height of a Tree :
  - the height of the root node or the depth of the deepest node.

- Degree of a Node :
  - The degree of a node is the total number of branches of that node.

- Forest :
  - A collection of disjoint trees is called a forest.

## Types of Tree
- Binary Tree
- Binary Search Tree
- AVL Tree
- B-Tree

## How can I reach any node in a Tree ? 
### In order to perform any operation on a tree, you need to reach to the specific node. The tree traversal algorithm helps in visiting a required node in the tree.


## Tree Applications
- Binary Search Trees(BSTs) are used to quickly check whether an element is present in a set or not.
- Heap is a kind of tree that is used for heap sort.
- A modified version of a tree called Tries is used in modern routers to store routing information.
- Most popular databases use B-Trees and T-Trees, which are variants of the tree structure we learned above to store their data
- Compilers use a syntax tree to validate the syntax of every program you write.


## Binary tree.

### A tree whose elements have at most two children is called a binary tree.

## What is the working principle of binary tree?
### A Binary tree is implemented with the help of pointers. The first node in the tree is represented by the root pointer. Each node in the tree consists of three parts, i.e., data, left pointer and right pointer