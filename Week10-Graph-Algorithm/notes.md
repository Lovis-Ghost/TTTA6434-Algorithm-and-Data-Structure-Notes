# Week 10: Graph Algorithm

## Topic Overview

This week introduces graph data structures and basic graph algorithms.

## Key Concepts

- A graph contains vertices and edges.
- Graphs can be directed or undirected.
- Graphs can be weighted or unweighted.
- Common graph representations are adjacency matrix and adjacency list.
- Breadth-first search and depth-first search are basic graph traversal methods.

## Step-by-step Explanation

1. Represent the graph using a suitable structure.
2. Choose a starting vertex.
3. Visit connected vertices.
4. Keep track of visited vertices.
5. Continue until all reachable vertices are processed.

## Time Complexity / Space Complexity

- BFS with adjacency list: `O(V + E)`.
- DFS with adjacency list: `O(V + E)`.
- `V` means number of vertices and `E` means number of edges.

## Python Example

```python
from collections import deque

def bfs(graph, start):
    visited = set([start])
    queue = deque([start])

    while queue:
        vertex = queue.popleft()
        print(vertex)
        for neighbor in graph[vertex]:
            if neighbor not in visited:
                visited.add(neighbor)
                queue.append(neighbor)

graph = {
    "A": ["B", "C"],
    "B": ["A", "D"],
    "C": ["A"],
    "D": ["B"]
}

bfs(graph, "A")
```

## Practice Questions

1. What is the difference between a vertex and an edge?
2. When should we use an adjacency list?
3. Compare BFS and DFS.

## My Reflection

Graphs are flexible because many real problems can be represented as connections. I need to practice choosing the correct graph representation.

