# Implementation of the PageRank algorithm in PySpark

The PageRank algorithm is used by Google search to rank web pages in their search engine.
PageRank is a link analysis algorithm and it assigns a numerical weighting to each element of a hyperlinked set of documents. Soruce node can point to any number of destination nodes.

1000 nodes in the ```graph-full.txt```, and m = 8192 edges, 1000 of which form a directed cycle (through all the nodes) which ensures that the graph is connected. It is easy to see that the existence of such a cycle ensures that there are no dead ends in the graph. There may be multiple directed edges between a pair of nodes. The first column in *graph-full.txt* refers to the source node, and the second column refers to the destination node.
