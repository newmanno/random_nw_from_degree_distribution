# Random_nw_from_degree_distribution
Creates a random network based off a previously known degree distribution

Input files:
  - csv file in the format of "Node_name, known_degree". Names of the columns can be anything.

Explanation of code:
This code takes as input a csv file containing the degree of each node in a known network one wants to compare to, then creates a random network by sampling from those degrees. For example, if the known network has a degree distribution like shown below, then the degree of the node in the random network would be drawn from that distribution. So many nodes should have a degree of 15 while fewer should have degrees of 5 or 25. In the end, the resulting random network will contain the same number of nodes as the known network, but number of edges may differ.

 40 |
 35 |
 30 |      __
 25 |   __|  |
 20 |  |  |  |__
 15 |__|  |  |  |
 10 |  |  |  |  |__
  5 |__|__|__|__|__|___
     05 10 15 20 25  
         Degree
