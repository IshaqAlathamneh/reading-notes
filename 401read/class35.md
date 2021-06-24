# Graphs
A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.


1. Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
1. Edge - An edge is a connection between two nodes.
1. Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
1. Degree - The degree of a vertex is the number of edges connected to that vertex.

### Directed vs Undirected
* An Undirected Graph is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.
* A Directed Graph also called a Digraph is a graph where every edge is directed.

### Complete vs Connected vs Disconnected
The three different types are completed, connected, and disconnected.

1. A complete graph is when all nodes are connected to all other nodes.
1. A connected graph is graph that has all of vertices/nodes have at least one edge.
1. A disconnected graph is a graph where some vertices may not have edges.


### Acyclic vs Cyclic
1. A cycle is when a node can be traversed through and potentially end up back at itself..
1. An acyclic graph is a directed graph without cycles.

### Graph Representation
1. Adjacency Matrix: An Adjacency matrix is represented through a 2-dimensional array. If there are n vertices, then we are looking at an n x n Boolean matrix
1. Adjacency List: An adjacency list is a collection of linked lists or array that lists all of the other vertices that are connected.

***a sparse graph is when there are very few connections. a dense graph is when there are many connections***