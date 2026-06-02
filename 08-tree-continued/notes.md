# Chapter 8: Tree Continued

# 第 8 章：树（续）

## 1. Key Idea / 核心思想

**English:**

This chapter continues tree topics, especially traversal and binary search tree operations.

**中文：**

这一章继续学习树，重点包括树的遍历和二叉搜索树操作。

## 2. Key Concepts / 关键概念

**English:**

- Preorder, inorder, and postorder are common traversal methods.
- In a binary search tree, smaller values are on the left and larger values are on the right.
- Inorder traversal of a binary search tree gives sorted output.

**中文：**

- 前序、中序和后序是常见的遍历方法。
- 在二叉搜索树中，较小的值在左边，较大的值在右边。
- 二叉搜索树的中序遍历会得到有序结果。

## 3. Step-by-step Explanation / 分步骤理解

**English:**

1. Choose the traversal order.
2. Visit the current node at the correct time.
3. Traverse the left subtree.
4. Traverse the right subtree.
5. Repeat until all nodes are visited.

**中文：**

1. 选择遍历顺序。
2. 在正确的时机访问当前节点。
3. 遍历左子树。
4. 遍历右子树。
5. 重复直到访问所有节点。

## 4. Simple Example / 简单例子

**English:**

```python
def inorder(node):
    if node is None:
        return
    inorder(node.left)
    print(node.value)
    inorder(node.right)
```

**中文：**

这个例子是中序遍历：先左子树，再当前节点，最后右子树。

## 5. My Understanding / 我的理解

**English:**

I can remember traversal by checking where the current node is visited.

**中文：**

我可以通过观察当前节点在什么时候被访问来记住遍历顺序。

## 6. Common Exam Points / 常见考点

**English:**

- Compare preorder, inorder, and postorder.
- Trace traversal output.
- Explain binary search tree search and insertion.

**中文：**

- 比较前序、中序和后序遍历。
- 手动写出遍历结果。
- 解释二叉搜索树的查找和插入。

