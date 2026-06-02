# Chapter 3: Algorithm Analysis II

# 第 3 章：算法分析（二）

## 1. Key Idea / 核心思想

**English:**

This chapter continues algorithm analysis with more patterns such as nested loops, logarithmic growth, and recursion.

**中文：**

这一章继续学习算法分析，包括嵌套循环、对数增长和递归等模式。

## 2. Key Concepts / 关键概念

**English:**

- Best case, average case, and worst case can be different.
- Nested loops often lead to `O(n^2)`.
- Algorithms that cut the problem in half often have `O(log n)`.
- Recursion may use extra stack memory.

**中文：**

- 最好情况、平均情况和最坏情况可能不同。
- 嵌套循环通常会得到 `O(n^2)`。
- 每次把问题减半的算法通常是 `O(log n)`。
- 递归可能会使用额外的调用栈空间。

## 3. Step-by-step Explanation / 分步骤理解

**English:**

1. Check whether the code has loops or recursion.
2. See how many times each part runs.
3. Focus on the part that grows the fastest.
4. Decide the final time and space complexity.

**中文：**

1. 先看代码是否有循环或递归。
2. 判断每一部分执行多少次。
3. 重点关注增长最快的部分。
4. 得出最终的时间和空间复杂度。

## 4. Simple Example / 简单例子

**English:**

```python
def count_pairs(numbers):
    count = 0
    for i in range(len(numbers)):
        for j in range(i + 1, len(numbers)):
            count += 1
    return count
```

This has nested loops, so the time complexity is about `O(n^2)`.

**中文：**

这个例子有嵌套循环，所以时间复杂度大约是 `O(n^2)`。

## 5. My Understanding / 我的理解

**English:**

I need to be careful when analyzing nested loops and recursive algorithms because the growth can become large quickly.

**中文：**

分析嵌套循环和递归时我需要特别小心，因为它们的增长可能很快变大。

## 6. Common Exam Points / 常见考点

**English:**

- Compare best, average, and worst case.
- Analyze nested loops.
- Explain why binary search is `O(log n)`.
- Understand recursion space usage.

**中文：**

- 比较最好、平均和最坏情况。
- 分析嵌套循环。
- 解释为什么二分查找是 `O(log n)`。
- 理解递归的空间使用。

