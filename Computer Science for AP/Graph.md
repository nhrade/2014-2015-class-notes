#Graph

Graph
	- Collection of nodes (vertices)  
	- Collection of edges  
	- Data is often associated with edges

Undirected Graph  
	- All edges are bidirectional

Directed Graphs (digraph)
	- All edges can only be traversed in one direction
	- Tree is a special case of a digraph  

2 different nodes (x, y) are adjacent if there is an edge from x to y.  
A path is a sequence of nodes in which each node is adjacent to the next one. 

length of path is # of edges traversed along the path.  

A cycle is a path len > 1 that begins & ends at the same node.  

A simple path is a path that contains no cycles.  

Degree of a node, is the number of edges in which the node is one of the end points.  

In Degree & Out Degree  
   - Used for directed graph.  
   - In Degree, number of edges I'm the dest.  
   - Out Degree, number of edges I'm the src.  

Neighboor of a node is the nodes that are adjacent to that node.  

Loop, a edge that is connected to itself.  

Underlying undirected graph
	   - If you take a digraph, and convert all edges to undirected.  

Connected, 2 nodes ar connected if there is a path from X to Y

Connected Component of a graph is the subgraph in which for  
every 2 nodes X and Y, X is connected to Y.