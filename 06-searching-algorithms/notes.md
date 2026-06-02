# Chapter 6: Searching Algorithms

# 第 6 章：查找算法

## 1. Key Idea / 核心思想

**English:**

Searching algorithms are used to find a target value in a collection of data.

**中文：**

查找算法用来在一组数据中寻找目标值。

## 2. Key Concepts / 关键概念

**English:**

- Linear search checks items one by one.
- Binary search works on sorted data.
- Linear search is simple but can be slow.
- Binary search is faster because it removes half of the search area each step.

**中文：**

- 线性查找会一个一个检查元素。
- 二分查找需要数据已经排序。
- 线性查找简单，但可能较慢。
- 二分查找更快，因为每一步都会减少一半查找范围。

## 3. Step-by-step Explanation / 分步骤理解

**English:**

1. Check whether the data is sorted.
2. Use linear search for unsorted data.
3. Use binary search for sorted data.
4. Stop when the target is found or no possible position remains.

**中文：**

1. 先判断数据是否已经排序。
2. 未排序数据可以用线性查找。
3. 已排序数据可以用二分查找。
4. 找到目标或没有可能位置时停止。

## 4. Simple Example / 简单例子

**English:**

```python
def binary_search(items, target):
    left = 0
    right = len(items) - 1

    while left <= right:
        mid = (left + right) // 2
        if items[mid] == target:
            return mid
        if items[mid] < target:
            left = mid + 1
        else:
            right = mid - 1

    return -1
```

**中文：**

这个例子是二分查找。每次检查中间元素，然后决定继续查找左边还是右边。

## 5. My Understanding / 我的理解

**English:**

I need to remember that binary search only works correctly when the data is sorted.

**中文：**

我需要记住二分查找只有在数据已经排序时才能正确使用。

## 6. Common Exam Points / 常见考点

**English:**

- Compare linear search and binary search.
- Explain why binary search is `O(log n)`.
- Trace binary search with left, right, and middle indexes.

**中文：**

- 比较线性查找和二分查找。
- 解释为什么二分查找是 `O(log n)`。
- 用 left、right 和 middle 手动追踪二分查找。

