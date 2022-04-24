# P6 Progress Log

## Apr. 18, 2022, 7:00PM

* Created the GitHub and progress log for the project.&#x20;

## Apr. 23, 2022, 8:00PM

* Created the skeleton class for the Graph, WeightedGraph, and their tester classes.
* Had some issues with what implementation i wanted to use and how i was going to execute it.&#x20;
* I chose to use an adjacency list, but was not sure how to implement it.&#x20;
  * My initial thought was to use and arraylist of arraylist\<Node>, but I realized how complicated traversing that could end up being, So i chose to somewhat follow the implementation shown in the lecture slides using an arraylist of nodes, and the nodes themselves having a linked list of neighbors.&#x20;
* Wrote the constructor
* Wrote a nodeExists() helper function
* Wrote the addNode method, and addNodes()
*   Wrote the addEdge method.&#x20;

    * I chose to make it ensure that the "from" node exists, but if the "to" node does not exist, it creates it and calls addEdge again. Doing this allows to keep a structured graph and allows for the creation of new nodes through addEdges

