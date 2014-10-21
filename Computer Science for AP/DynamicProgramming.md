#Dynamic Programming

##Dijkstra's Algorithm

Distance list is the shortest path h to every node.

init dist list
 - start node dist = 0
 - all other nodes dist = infinity

while dist !isEmpty() & dest not in perma  
 - take smallest node out of dist(infinity)
 - move a to perm  
 - for each neighbor of a
  *compute dist toa + dist to neighbor
  if this dist < dist list entry update


Is a greedy algorithm
 - Look at current data and do best move
 - Don't check all possible solutions

Graph Coloring
 - Any 2 nodes that have an edge between them to have the same color.
 - is a 2^n problem
