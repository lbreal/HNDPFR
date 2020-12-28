These folders contain the randomly created data set for the Multimodal Hub Network Design Problem with Flexible Routes. 
The files are divided according to the potential economies of scale obtained when using a larger vehicle when it is fully utilized (alpha).

The data file format is as follows:
<r>					Total number of available vehicle type
<tau[1]> <speed[1]> <b[1]> <a[1]> 	Capacity, speed, fixed operating cost, fixed acquisition cost for vehicles of type 1 
  :         :             :
  :         :             :
<tau[r]> <speed[r]> <b[r]> <a[r]> 	Capacity, speed, fixed operating cost, fixed acquisition cost for vehicles of type r
<n>                                     Number of nodes
<h[1]>					Fixed cost for installing a hub in node 1
:
:
<h[n]>					Fixed cost for installing a hub in node n
<x[1]> <y[1]>                           x & y coordinates of node 1
  :
  :
<x[n]> <y[n]>                           x & y coordinates of node n
1 1 <w[1][1]> <dist[1][1]>              demand from node 1 to node 1 and distance between node 1 and node 1
  :         :             :
  :         :             :
n n <w[n][n]> <dist[n][n]>              demand from node n to node n and distance between node n and node n

The fixed operating cost is multiplied by a factor of ten.
The distance values are rounded upward.
For every origin i and destination j, such that i != j, if w[i][j] = 0, we change it for 1.

