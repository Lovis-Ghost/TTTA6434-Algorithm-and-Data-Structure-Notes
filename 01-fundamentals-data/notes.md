# Chapter 1: Fundamentals of Data

# 第 1 章：数据基础

## 1. Key Idea / 核心思想

**English:**

An algorithm is a series of clear step-by-step instructions for processing data and solving a problem. A data structure is a way to store and organize data so the program can use it efficiently.

A simple way to remember this chapter is:

```text
Program = Algorithms + Data Structures
```

**中文：**

算法是一组清楚的步骤，用来处理数据并解决问题。数据结构是用来存储和组织数据的方法，让程序可以更有效地使用数据。

这一章可以用一句话来记：

```text
程序 = 算法 + 数据结构
```

## 2. Key Concepts / 关键概念

**English:**

- Data is the information used by a program.
- An algorithm explains what steps the program should follow.
- A data structure explains how data is stored and organized.
- Algorithm analysis is important because time and memory resources are limited.
- If the data is very large, a poor algorithm or unsuitable data structure may make the program very slow or even fail.
- Linear data structures include arrays, linked lists, stacks, and queues.
- Non-linear data structures include trees and graphs.

**中文：**

- 数据是程序使用的信息。
- 算法说明程序应该按照什么步骤执行。
- 数据结构说明数据应该怎样存储和组织。
- 算法分析很重要，因为时间和内存资源都是有限的。
- 如果数据量很大，不好的算法或不合适的数据结构会让程序变慢，甚至运行失败。
- 线性数据结构包括数组、链表、栈和队列。
- 非线性数据结构包括树和图。

## 3. Step-by-step Explanation / 分步骤理解

**English:**

1. First, understand what data the problem needs.
2. Then, choose a suitable data structure to store the data.
3. Next, design an algorithm to process the data.
4. After that, think about time efficiency and space efficiency.
5. Finally, check whether the structure is suitable for the problem.

**中文：**

1. 先理解题目需要处理什么数据。
2. 然后选择合适的数据结构来存储数据。
3. 接着设计一个算法来处理这些数据。
4. 之后考虑时间效率和空间效率。
5. 最后判断这个数据结构是否适合当前问题。

## 4. Simple Example / 简单例子

**English:**

Array-like list in Python:

```python
numbers = [10, 20, 30, 40]
print(numbers[0])
print(numbers[2])
```

Stack using list:

```python
stack = []
stack.append("A")  # push
stack.append("B")  # push
print(stack[-1])   # peek
print(stack.pop()) # pop
```

Queue using `deque`:

```python
from collections import deque

queue = deque()
queue.append("A")      # enqueue
queue.append("B")      # enqueue
print(queue.popleft()) # dequeue
```

**中文：**

Python 的 list 可以像数组一样通过下标访问元素。栈可以用 list 的 `append` 和 `pop` 实现。队列可以用 `collections.deque`，因为它从队头删除元素比较方便。

## 5. My Understanding / 我的理解

**English:**

The most important part for me is choosing between an array and a linked list. An array uses continuous memory and gives fast random access by index, but insertion and deletion may be slow because elements may need to move. A linked list does not use continuous memory. Its nodes are connected by pointers, so insertion and deletion can be easier, but direct access is slower.

Stack follows LIFO, which means Last In, First Out. Queue follows FIFO, which means First In, First Out.

**中文：**

我觉得最重要的是学会在不同问题中选择数组还是链表。数组使用连续内存，可以快速通过下标访问元素，但是插入和删除可能比较慢，因为元素可能需要移动。链表不需要连续内存，它通过指针连接节点，所以插入和删除可能更方便，但是不能快速直接访问某个位置。

栈遵循 LIFO，也就是后进先出。队列遵循 FIFO，也就是先进先出。

## 6. Common Exam Points / 常见考点

**English:**

- Explain what an algorithm is.
- Explain what a data structure is.
- Explain `Program = Algorithms + Data Structures`.
- Compare linear and non-linear data structures.
- Compare array and linked list.
- Explain LIFO for stack and FIFO for queue.
- Know stack operations: push, pop, peek.
- Know queue operations: enqueue, dequeue.

**中文：**

- 解释什么是算法。
- 解释什么是数据结构。
- 解释 `程序 = 算法 + 数据结构`。
- 比较线性和非线性数据结构。
- 比较数组和链表。
- 解释栈的后进先出和队列的先进先出。
- 记住栈的操作：push、pop、peek。
- 记住队列的操作：enqueue、dequeue。

