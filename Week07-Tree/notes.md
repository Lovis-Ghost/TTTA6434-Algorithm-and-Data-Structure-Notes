# Week 07: Tree

## Topic Overview

This week introduces tree data structures and basic tree terms.

## Key Concepts

- A tree is a hierarchical data structure.
- A node stores data.
- The root is the top node.
- A child is below another node.
- A leaf has no children.
- A binary tree has at most two children for each node.

## Step-by-step Explanation

1. Start from the root node.
2. Follow edges to reach child nodes.
3. Identify parent, child, sibling, and leaf nodes.
4. Use traversal methods to visit nodes.

## Time Complexity / Space Complexity

- Visiting all nodes in a tree is `O(n)`.
- Searching in a balanced binary search tree is `O(log n)`.
- Searching in an unbalanced tree can become `O(n)`.

## Python Example

```python
class Node:
    def __init__(self, value):
        self.value = value
        self.left = None
        self.right = None

root = Node(10)
root.left = Node(5)
root.right = Node(15)

print(root.value)
```

## Practice Questions

1. What is the root of a tree?
2. What is the difference between a leaf and an internal node?
3. Why can a balanced tree search be faster?

## My Reflection

Trees are useful for representing hierarchy. I need to practice drawing trees because it makes the structure easier to understand.

