# Week 01: Fundamentals of Data

## Topic Overview

This week introduces the basic ideas of algorithms and data structures. An algorithm is a step-by-step procedure that solves a problem. A data structure is a way to store and organize data efficiently.

In programming, both ideas are connected. A useful way to remember this is:

```text
Program = Algorithms + Data Structures
```

The algorithm tells the program what steps to follow, while the data structure helps the program manage the data.

## Key Concepts

- Data is the information used by a program.
- An algorithm is a clear set of instructions for processing data and solving a problem.
- A data structure stores and organizes data so the program can use it properly.
- Algorithm analysis is important because memory and time resources are limited.
- If the data is very large, a slow algorithm or unsuitable data structure can make a program slow or even fail.
- Time efficiency means how fast an algorithm runs.
- Space efficiency means how much memory an algorithm or data structure uses.

## Q&A Summary

**Q1: What is an algorithm?**

An algorithm is a series of clear instructions. It explains how to process data step by step to solve a problem.

**Q2: What is a data structure?**

A data structure is used to store and organize data. It helps the program access and manage data more efficiently.

**Q3: Why do we need to analyze algorithms?**

We need to analyze algorithms because computer memory and processing resources are limited. If the input data is very large, an inefficient algorithm may cause the server or program to become very slow or fail.

**Q4: What are linear and non-linear data structures?**

Linear data structures store data in a sequence. Examples include arrays, linked lists, stacks, and queues.

Non-linear data structures do not store data in one straight sequence. Examples include trees and graphs.

**Q5: What is the difference between an array and a linked list?**

An array uses continuous memory space. A linked list does not need continuous memory because its nodes are connected using pointers.

**Q6: What is a stack?**

A stack is a linear data structure that follows LIFO, which means Last In, First Out.

**Q7: What is a queue?**

A queue is a linear data structure that follows FIFO, which means First In, First Out.

**Q8: What is the most important point from this topic?**

The most important point is learning how to choose between an array and a linked list in different problems.

## Array vs Linked List

| Feature | Array | Linked List |
| --- | --- | --- |
| Memory | Uses continuous memory space | Nodes are not stored continuously |
| Connection | Items are stored beside each other | Nodes are connected by pointers |
| Access | Fast random access by index | Direct access is slower |
| Insertion and deletion | May be slow because items may need to shift | Can be easier if the position is known |
| Best use | When we need fast access by index | When we need many insertions and deletions |

An array is useful when I want to quickly access an item using its index. For example, getting the first or third item is fast.

A linked list is useful when I need to insert or delete data often. However, if I want to find a specific item, I may need to move through the nodes one by one.

## Stack and Queue

### Stack

A stack follows **LIFO**, which means **Last In, First Out**. The last item added will be the first item removed.

Common stack operations:

- `push`: add an item to the top of the stack.
- `pop`: remove the top item from the stack.
- `peek`: look at the top item without removing it.

Example idea: a stack of plates. The last plate placed on top is usually the first plate taken.

### Queue

A queue follows **FIFO**, which means **First In, First Out**. The first item added will be the first item removed.

Common queue operations:

- `enqueue`: add an item to the back of the queue.
- `dequeue`: remove an item from the front of the queue.

Example idea: people lining up at a counter. The first person in the line is served first.

## Simple Python Examples

### List as an Array-like Structure

Python lists can be used like arrays because we can access items using an index.

```python
numbers = [10, 20, 30, 40]

print(numbers[0])
print(numbers[2])
```

### Stack Using List

```python
stack = []

stack.append("A")  # push
stack.append("B")  # push
stack.append("C")  # push

print(stack[-1])   # peek
print(stack.pop()) # pop
print(stack)
```

### Queue Using collections.deque

```python
from collections import deque

queue = deque()

queue.append("A")      # enqueue
queue.append("B")      # enqueue
queue.append("C")      # enqueue

print(queue.popleft()) # dequeue
print(queue)
```

## Practice Questions

1. What is the meaning of `Program = Algorithms + Data Structures`?
2. Why is algorithm analysis important when the input data is large?
3. What is the difference between a linear and non-linear data structure?
4. Compare array and linked list in terms of memory and access speed.
5. What is the difference between LIFO and FIFO?

## My Reflection

From this topic, I understand that algorithms and data structures work together in a program. I also learned that choosing the correct data structure is important because memory and time are limited. The part I need to focus on more is deciding when to use an array and when to use a linked list for different problems.
