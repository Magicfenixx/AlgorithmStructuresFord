AlgorithmStructuresFord

The Bellman–Ford algorithm is an algorithm that computes shortest paths from a single source vertex to all of the other vertices in a weighted digraph.
It is slower than Dijkstra's algorithm for the same problem, but more versatile, as it is capable of handling graphs in which some of the edge weights are negative numbers.

Negative edge weights are found in various applications of graphs. This is why this algorithm is useful.
If a graph contains a "negative cycle" (i.e. a cycle whose edges sum to a negative value) that is reachable from the source, then there is no cheapest path: 
any path that has a point on the negative cycle can be made cheaper by one more walk around the negative cycle. 
In such a case, the Bellman–Ford algorithm can detect and report the negative cycle.
