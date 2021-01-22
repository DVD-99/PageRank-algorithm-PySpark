# Implementation of the PageRank algorithm in PySpark

The PageRank algorithm is used by Google search to rank web pages in their search engine.
PageRank is a link analysis algorithm and it assigns a numerical weighting to each element of a hyperlinked set of documents. Soruce node can point to any number of destination nodes.

![Page_Rank Img](https://github.com/DVD-99/PageRank-algorithm-PySpark/blob/main/PageRanks-Example.jpg)

**Node B** has more weight in the above image than other nodes as many nodes are pointing to B. In **C's case**, even though only one node is pointing to it, B has a considerable weight, which increases C's weight.

1000 nodes in the ```graph-full.txt```, and m = 8192 edges, 1000 of which form a directed cycle (through all the nodes, assume graph has no dead-ends) which ensures that the graph is connected. It is easy to see that the existence of such a cycle ensures that there are no dead ends in the graph. There may be multiple directed edges between a pair of nodes. The first column in *graph-full.txt* refers to the source node, and the second column refers to the destination node.

These are the weights of the top 5 nodes.
```
263:0.0020202911815182184 
537:0.0019433415714531497 
965:0.0019254478071662631 
243:0.001852634016241731 
285:0.0018273721700645144
```

If you want to experiment, use ```graph-small.txt```
