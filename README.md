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



Time Spent: 1 hr (10% mark)

## Apr. 24, 2:00PM

* Found a bug in my addEdge method that came from a helper method from my node class.&#x20;
  * I was searching for a node with name x inside neighbors instead of the graph, which resulted in a nullpointerexception.
* Wrote addEdges method
* Wrote removeNode method
  * removed the node from the arraylist and then iterated through the graph to remove any references to the node in all of the nodes neighbors list.&#x20;
* Wrote printGraph()
* Started writing read() method.
  * Decided to use a buffered reader for each line, and then use the string split function to create a string array with all the node names.&#x20;
  * I then used that array to first create the main node, and then added its edges with the addEdges function.

Time Spent: 1 hr (50% mark)

## Apr. 24, 2022, 4:00PM

* Started writing the GraphTester class methods.
  * Wrote testing methods for all methods up to the read method.
* Started working on the path searching methods
  * Struggled with getting the DFS method working correctly for a while.
    * I have it to the point that it returns a somewhat correct path for longer paths. It is still including some dead end nodes that have been visited. And for shorter ones it just returns a alot of extra nodes.&#x20;

Time Spent: 3 hr (Actual 50% mark)
