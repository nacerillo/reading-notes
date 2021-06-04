# Class 35 Notes: Graphs:

**Definition:** a non-linear data structure that is made up of a finite amount of nodes/verticies connected by a finite amount of edges.

- **vertex:** the nodes of a graph, each containing both a scrap of data, and references to its neighbors.
- **edge:** a connecting point between two vertices.
- **neighbor:** a vertex that shares an edge with another vertex.
- **degree:** used to describe the number of edges that are connected to a vertex.

## Types of graphs:

- Directed Graph/Digraph: every edge has a single direction. kind of like a linked list.
- Undirected Graph: edges have not direction. connections can go both ways.

- Complete Graphs: all nodes/vertices are connected to all other nodes/verticies.
- Connected Graphs: all nodes share at least one edge with another node.
- Disconnected: some nodes do not have edges. Not all nodes are connected.

- Cyclic Graph: A graph who's connecting adges/nodes make a cycle or loop.
- Acyclic Graph: A graph that does NOT form a cycle or loop.

## Ways of representing a Graph:

- Adjacency Matrix. a two - dimensional array.
- Adjacency List. a collection of linked-lists or arrays.
