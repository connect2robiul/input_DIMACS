import re
import networkx as nx
import numpy
import random
def hasNumbers(inputString):
    return any(char.isdigit() for char in inputString)

G_Row=list()
G_Column=list()
with open('myciel3.col', 'r') as f:
    for l in f:
        x, *y = l.split()
        if hasNumbers(y):
            m,n = re.findall('\d+', l ) 
            G_Row.append(int(m))
            G_Column.append(int(n))
Node = G_Row.pop(0)
Edge = G_Column.pop(0)
graph=nx.Graph()

for i in range(1,Node+1):
    graph.add_node(i)
for i in range(Edge):
    graph.add_edge(G_Row[i],G_Column[i])
print(graph.node)
print(graph.edge)
