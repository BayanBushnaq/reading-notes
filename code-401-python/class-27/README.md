# Graphs
## A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.

### Here is some common terminology used when working with Graphs:

 - Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
 - Edge - An edge is a connection between two nodes.
 - Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
 - Degree - The degree of a vertex is the number of edges connected to that vertex.

 ## Types of Graphs : 
  - Directed :  is a graph where every edge is directed.
  -  Undirected :  is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.
  - Complete : A complete graph is when all nodes are connected to all other nodes.
  - Connected : A connected graph is graph that has all of vertices/nodes have at least one edge.
  - Disconnected :  is a graph where some vertices may not have edges.
  - Acyclic  : is a directed graph without cycles.

        * A cycle is when a node can be traversed through and potentially end up back at itself.
  - Cyclic : A Cyclic graph is a graph that has cycles.

        * A cycle is defined as a path of a positive length that starts and ends at the same vertex.

## Graph Representation
### We represent graphs through:

    * Adjacency Matrix

    * Adjacency List

## Traversals
### You will be required to traverse through a graph. The traversals itself are like those of trees.

-  Breadth First method: The breadth first traversal of a graph is like that of a tree, with the exception that graphs 
    can have cycles. 
- Depth first : the depth first traversal uses a Stack to visit all children of a given subtree.

## Tree vs Graphs: 

![Tree vs Graph](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRzvN1eDEEHg_PVpjxev7CtVPpDTYfrkRVgSg&usqp=CAU)