# Chapter 10: Graph Algorithm

# 第 10 章：图算法

## 1. Key Idea / 核心思想

**English:**

A graph is a data structure used to represent relationships and connections.

**中文：**

图是一种用来表示关系和连接的数据结构。

## 2. Key Concepts / 关键概念

**English:**

- A vertex is a node in a graph.
- An edge connects two vertices.
- Graphs can be directed or undirected.
- Graphs can be weighted or unweighted.
- BFS and DFS are common graph traversal algorithms.

**中文：**

- 顶点是图中的节点。
- 边连接两个顶点。
- 图可以是有向图或无向图。
- 图可以是有权图或无权图。
- BFS 和 DFS 是常见的图遍历算法。

## 3. Step-by-step Explanation / 分步骤理解

**English:**

1. Represent the graph using an adjacency list or matrix.
2. Choose a starting vertex.
3. Visit connected vertices.
4. Mark visited vertices.
5. Continue until all reachable vertices are processed.

**中文：**

1. 用邻接表或邻接矩阵表示图。
2. 选择起始顶点。
3. 访问相连的顶点。
4. 标记已经访问过的顶点。
5. 重复直到处理完所有可到达的顶点。

## 4. Simple Example / 简单例子

**English:**

```python
from collections import deque

def bfs(graph, start):
    visited = {start}
    queue = deque([start])
    while queue:
        vertex = queue.popleft()
        print(vertex)
        for neighbor in graph[vertex]:
            if neighbor not in visited:
                visited.add(neighbor)
                queue.append(neighbor)
```

**中文：**

这个例子是 BFS。它使用队列，从起点开始一层一层访问相邻顶点。

## 5. My Understanding / 我的理解

**English:**

Graphs are useful because many real problems can be described as connections.

**中文：**

图很有用，因为很多现实问题都可以表示成连接关系。

## 6. Common Exam Points / 常见考点

**English:**

- Explain vertex and edge.
- Compare adjacency list and adjacency matrix.
- Trace BFS and DFS.
- Know `O(V + E)` for traversal with adjacency list.

**中文：**

- 解释顶点和边。
- 比较邻接表和邻接矩阵。
- 手动追踪 BFS 和 DFS。
- 记住邻接表遍历通常是 `O(V + E)`。

