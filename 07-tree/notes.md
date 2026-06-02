# Chapter 7: Tree

# 第 7 章：树

## 1. Key Idea / 核心思想

**English:**

A tree is a non-linear data structure used to represent hierarchical relationships.

**中文：**

树是一种非线性数据结构，用来表示层级关系。

## 2. Key Concepts / 关键概念

**English:**

- The root is the top node.
- A parent node can have child nodes.
- A leaf node has no children.
- A binary tree has at most two children for each node.

**中文：**

- 根节点是最上面的节点。
- 父节点可以有子节点。
- 叶子节点没有子节点。
- 二叉树中每个节点最多有两个子节点。

## 3. Step-by-step Explanation / 分步骤理解

**English:**

1. Start from the root.
2. Follow edges to child nodes.
3. Identify parent, child, sibling, and leaf nodes.
4. Use traversal to visit nodes.

**中文：**

1. 从根节点开始。
2. 沿着边找到子节点。
3. 判断父节点、子节点、兄弟节点和叶子节点。
4. 使用遍历方法访问节点。

## 4. Simple Example / 简单例子

**English:**

```python
class Node:
    def __init__(self, value):
        self.value = value
        self.left = None
        self.right = None

root = Node(10)
root.left = Node(5)
root.right = Node(15)
```

**中文：**

这个例子建立了一个简单二叉树，根节点是 10，左子节点是 5，右子节点是 15。

## 5. My Understanding / 我的理解

**English:**

Trees are easier to understand when I draw the nodes and connections.

**中文：**

画出节点和连接关系后，树结构会更容易理解。

## 6. Common Exam Points / 常见考点

**English:**

- Identify root, parent, child, and leaf nodes.
- Explain binary tree.
- Understand basic tree traversal ideas.

**中文：**

- 判断根节点、父节点、子节点和叶子节点。
- 解释二叉树。
- 理解树遍历的基本思想。

