# Week 08: Tree Continued

## Topic Overview

This week continues tree topics, including traversal and binary search tree operations.

## Key Concepts

- Tree traversal means visiting each node.
- Common traversals are preorder, inorder, and postorder.
- In a binary search tree, smaller values are usually on the left and larger values are on the right.

## Step-by-step Explanation

1. Choose the traversal method.
2. Visit the current node based on the traversal order.
3. Move to the left subtree.
4. Move to the right subtree.
5. Repeat until all nodes are visited.

## Time Complexity / Space Complexity

- Tree traversal is `O(n)` time.
- Recursive traversal uses stack space, usually `O(h)` where `h` is tree height.
- Binary search tree insert and search are `O(log n)` if balanced.

## Python Example

```python
def inorder(node):
    if node is None:
        return
    inorder(node.left)
    print(node.value)
    inorder(node.right)
```

## Practice Questions

1. What is inorder traversal?
2. Why does inorder traversal of a binary search tree give sorted output?
3. What happens if a binary search tree becomes unbalanced?

## My Reflection

Tree traversal is easier when I remember the position of "visit node" in the order. I should practice preorder, inorder, and postorder with drawings.

