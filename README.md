# Warehouse Delivery Network using Comb Sort, Kruskal's algorithm, and Treap

## Introduction of Algorithms
### Comb sort
- Comparison based sorting system.
- An improvement on bubble sort - allows for swaps of non adjacent elements.
- A “turtle” is a small element located towards the end of an array.
- Comb sort removes all the “turtle” values or small values near the end of the list.

### Treap 
- The name is a blend of tree and heap
- Used to solve connectivity problems
- Similar to binary search tree
- Made to solve the problem of imbalance
- Definition: A treap is a combination of a binary search tree, and a hea
- Goal is to construct a balanced tree, meaning each parent node on both the right and left side has roughly the same child nodes
- Treaps assign a randomly generated “priority” number to each of the nodes, tree is then constructed as if it is a heap, with the highest priority being at the top . This creates a balanced tree, meaning the worst case is usually avoided.

### Kruskal's algorithm
- Developed to solve the problem of finding the minimum spanning tree of a connected undirected graph
- Practical solution to many problems such as minimizing cost or total distance between a set of locations
- Finds a minimum spanning forest of an undirected edge-weighted graph. If the graph is connected, it finds a minimum spanning tree
- It is a greedy algorithm that in each step adds to the forest the lowest-weight edge that will not form a cycle
- The key steps of the algorithm are sorting and the use of a disjoint-set data structure to detect cycles

## Microcosm
- To reach the most clients with a product, businesses tend to send out their product using their own specialized delivery network that sorts each neighborhood based on how far away they are from the warehouse to effectively send the 
product in the most time and cost efficient manner. 
To do this, the business will need to sort the neighborhoods based on the distance between the warehouse and the neighborhoods, which Kruskal algorithm can use alongside the comb sort method
- When they store their neighborhoods in their system, they also need to have a way to sort the orders of the customers in said neighborhoods, which can be stored using the treap data structure

## Functionality
- Demonstrate the use of Kruskal's algorithm to find the MST of a graph of neighborhoods and uses Comb Sort to sort them into the graph
- Uses Treap to efficiently search through package codes

## Usage Instructions
- Create a text file with the first line containing two integers being the number of edges (roads) and vertices (neighborhoods)
- The rest of the lines will contain: the first integer is the source virtice, second integer is the destination, the third weight is the weight (distance)

## Dependencies
- Depends on one text file in a specific format

## Installation Instructions
- Download the folder which contains every file required, including a test text file
