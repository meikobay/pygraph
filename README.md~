# pygraph
> graph for python which contain the Dijkstra algorithm to calculate the shortest path given a start and end node on the built graph.


## install
git clone https://github.com/huyanmingtoby/pygraph.git

```python
cd ~/pygraph-1.0
sudo python setup.py install
```

## An example

![graph example](https://github.com/huyanmingtoby/pygraph/blob/master/20190404124648480.png)

```python
from pygraph.pygraph import Graph
from pygraph.pygraph import Edge
g = Graph()
gmat = {}
gmat[0] = {1:4, 2:5}
gmat[1] = {0:4, 3:2, 4:3, 5:6}
gmat[2] = {0:5, 4:8, 5:7, 6:7}
gmat[3] = {1:2, 7:5, 8:8}
gmat[4] = {1:3, 2:8, 7:4, 8:5}
gmat[5] = {1:6, 2:7, 8:3, 9:4}
gmat[6] = {2:7, 8:8, 9:4}
gmat[7] = {3:5, 4:4, 10:3, 11:5}
gmat[8] = {3:8, 4:5, 5:4, 6:8, 10:6, 11:2}
gmat[9] = {5:4, 6:4, 10:1, 11:3}
gmat[10] = {7:3, 8:6, 9:1, 12:4}
gmat[11] = {7:5, 8:2, 9:3, 12:3}
gmat[12] = {10:4, 11:3}
for key_i in gmat.keys():
    for key_j in gmat[key_i].keys():
        e = Edge(key_i, key_j, gmat[key_i][key_j])
        g.add_edge(e)

print(g.find_shortest_path(0, 12))

```

output:
shortest_path = [0, 1, 4, 8, 11, 12]
path_dist = 17
