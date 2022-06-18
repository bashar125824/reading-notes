# What is Graphs ?

***A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.***

*Here is some common terminology used when working with Graphs:*

- **Vertex** - *A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.*

- **Edge** - *An edge is a connection between two nodes.*

- **Neighbor** - *The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.*

- **Degree** - *The degree of a vertex is the number of edges connected to that vertex.*

# Directed vs Undirected Graphs

## Undirected Graphs

***An Undirected Graph is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.***

***For example, in the graph below, Node C is connected to Node A, Node E and Node B. There are no “directions” given to point to specific vertices. The connection is bi-directional.***

![IMG](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/UndirectedGraph.PNG)

## Directed Graphs (Digraph)

***A Directed Graph also called a Digraph is a graph where every edge is directed.***

***Unlike an undirected graph, a Digraph has direction. Each node is directed at another node with a specific requirement of what node should be referenced next.***

![IMG](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/DirectedGraph.PNG)

# Acyclic vs Cyclic Graphs

## Acyclic Graph

***An acyclic graph is a directed graph without cycles.***

***A cycle is when a node can be traversed through and potentially end up back at itself.***

*Here is an example of 3 acyclic graphs:*

![img](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/threeAcyclic.png)

## Cyclic Graphs

***A Cyclic graph is a graph that has cycles.***

***A cycle is defined as a path of a positive length that starts and ends at the same vertex.***

*Here is an example of a two different cyclic graph:*

![img](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/cyclic.PNG)

# Types of Graghs ( Complete vs Connected vs Disconnected )

## Complete Graphs

***A complete graph is when all nodes are connected to all other nodes.***

![img](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/CompleteGraph.PNG)

## Connected Graphs

***A connected graph is graph that has all of vertices/nodes have at least one edge.***

![IMG](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/ConnectedGraph.PNG)

## Disconnected Graphs 

***A disconnected graph is a graph where some vertices may not have edges.***

![img](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/DisconnectedGraph.PNG)


# Graph Representation

*We represent graphs through:*

- **Adjacency Matrix**
- **Adjacency List**
