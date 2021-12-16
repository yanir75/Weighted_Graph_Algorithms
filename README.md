# Weighted Directed Graphs
## Assignment 2 - Object Oriented Programming 
**Netanel Levine**   
**Yanir Cohen**    
--- 
This project is about simulating and illustrating algorithms on graphs. In this project we will load graphs from Json files and will activate specific algorithms on those graphs. In addition we will create a UI that illustrates the algorithm we activated on the graph.
In this way you will be able to load and activate algorithm on the graphs as you wish.
 
---
## Project UML

<img src="https://github.com/netanellevine/Weighted_Graph_Algorithms/blob/main/uml/Arcithecture.png">
---

## Structure  

Our project structure
1. Node, Node represents a significant place in our university i.e building,market etc.
Each node holds information regarding itself, street name, tag etc.    
3. Location , GeoLocation represents the real life (latitude and longitude).    
5. Edge , Edge resembles a way of trasport (road,sidewalk etc) between two nodes.  
Edges contain information as well for example road 4 ,etc.
Not all edges are two way edges. Because there are one way roads.
In addition the cost of each edge is not the same for similar reasons.

## Graph:
Graph is built upon founded on those.
Graph contains all the nodes and all the edges in a given place, nodes can be added and removed, same goes for edges.  
Through it we will represent a small area with places of significance and a way to modify them quickly providing elasticity.

## Algorithms:
Algorithms are the main event over here. As can be seen this graph can represent real life places.
As so we would like the best way from a node to another node, this will be done by calculating the best way through each edges from each node. This will be done with Shortest path.
In addition we would like to know the time of each trip, as for we can retrieve the cost of the way from one node to another. This will be done with Shortest path dist.
Moreover we would like to know the best way between one node with a few stops on the way. This will be done through the best effor TSP.
At last we would like to know the center of the place, which place is probably closest to all. This will be done through Center.
Those are the main functions we will use to represent as closely as possible real life situations.  

## Gui:
Finally, we would like a visualistic way to show the users the graph, edges, best roads etc.  
As a result we created user interface which will visualize the graph and algorithms mentioned above.  
It will display the nodes and edges between all the nodes. Algorithms will be easily activated to illustrate the situations.  
This will be a user friendly gui which aspires to be easy to use, adjustable and illustrate our project as best as we can.
In conclusion, you will be able to see the way and understand much better what is the best result for your request.

## Results
Here are the results of the algorithm on a connected graph.  
The left column has the function we activated. The first row has the number of nodes.
|        | **1000/20000** | **10000/200000** | **100000/2000000** | **1000000/200000000** |
|-----------|--------|--------|--------|--------|
|**is Connected**|	0.01s	 | 0.2s  |	 5-17s  | NULL  | 
|**TSP 10 Nodes** |0.02s	 | 0.5-1s   |	1-10s  | NULL  | 
|**Center** |2s	 | 5.5m   |	NULL   | NULL  | 
|**Shortest Path** |0.02s | 0.04s   |	5s   | NULL  | 
  
We are able to generate a graph with 1mk nodes and 20mk edges but are unable to run any algorithm on it, due to heap space.
The results vary depends on how th graph is generated.

---
## Gui 
Here we attached a picture of the gui.
Each button will activate a different algorithm.
<div align="center">
    <img src="https://github.com/netanellevine/Weighted_Graph_Algorithms/blob/main/gui/graph.PNG">
 </div>
---

## How to use
will be done soon

---
## Sources:

  - <a href="https://www.youtube.com/watch?v=CerlT7tTZfY&t">Djikstra's algorithm using a priority queue - Youtube</a>
  - <a href="https://www.geeksforgeeks.org/connectivity-in-a-directed-graph/">Check if a graph is strongly connected</a>
