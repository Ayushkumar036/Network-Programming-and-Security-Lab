# Distance Vector Routing Algorithm using Bellman Ford's Algorithm

## Description

A distance-vector routing protocol in data networks determines the best route for data packets based on distance. Distance-vector routing protocols measure the distance by the number of routers a packet has to pass, one router counts as one hop.
## Working

1) This step initializes distances from the source to all vertices as infinite and distance to the source itself as 0.    
   Create an array dist[] of size |V| with all values as infinite except dist[src] where src is source vertex.  

2) This step calculates shortest distances. Do following |V|-1 times where |V| is the number of vertices in given graph.  
   a) Do following for each edge u-v   
      If dist[v] > dist[u] + weight of edge uv, then update dist[v]    
        dist[v] = dist[u] + weight of edge uv    


## Output

![Output 1](https://github.com/Ayushkumar036/Network-Programming-and-Security-Lab/blob/main/Routing-BellmanFord/output1.PNG?raw=true)  
![Output 2](https://github.com/Ayushkumar036/Network-Programming-and-Security-Lab/blob/main/Routing-BellmanFord/output2.PNG?raw=true)
