# Chapter 2: Algorithm Analysis I

# 第 2 章：算法分析（一）

## 1. Key Idea / 核心思想

**English:**

Algorithm analysis helps us understand how efficient an algorithm is when the input size becomes larger.

**中文：**

算法分析帮助我们理解当输入规模变大时，一个算法是否有效率。

## 2. Key Concepts / 关键概念

**English:**

- Time complexity describes how running time grows.
- Space complexity describes how memory usage grows.
- Big O notation is used to describe the growth rate.
- Common examples include `O(1)`, `O(n)`, and `O(n^2)`.

**中文：**

- 时间复杂度描述运行时间如何增长。
- 空间复杂度描述内存使用如何增长。
- Big O 记号用来表示增长速度。
- 常见例子包括 `O(1)`、`O(n)` 和 `O(n^2)`。

## 3. Step-by-step Explanation / 分步骤理解

**English:**

1. Find the main operation in the algorithm.
2. Count how many times it runs.
3. Ignore small constants.
4. Keep the most important growth term.
5. Write the result using Big O notation.

**中文：**

1. 找出算法中的主要操作。
2. 计算这个操作大概执行多少次。
3. 忽略较小的常数。
4. 保留最重要的增长项。
5. 用 Big O 记号表示结果。

## 4. Simple Example / 简单例子

**English:**

```python
def find_max(numbers):
    largest = numbers[0]
    for number in numbers:
        if number > largest:
            largest = number
    return largest
```

This function checks each number once, so the time complexity is `O(n)`.

**中文：**

这个函数会检查每一个数字一次，所以时间复杂度是 `O(n)`。

## 5. My Understanding / 我的理解

**English:**

I understand that Big O is not the exact running time. It is a way to describe how the algorithm grows when the input becomes larger.

**中文：**

我理解 Big O 不是精确的运行时间，而是用来描述输入变大时算法增长情况的方法。

## 6. Common Exam Points / 常见考点

**English:**

- Explain time complexity and space complexity.
- Identify `O(1)`, `O(n)`, and `O(n^2)`.
- Analyze simple loops.
- Explain why constants are ignored in Big O.

**中文：**

- 解释时间复杂度和空间复杂度。
- 判断 `O(1)`、`O(n)` 和 `O(n^2)`。
- 分析简单循环。
- 解释为什么 Big O 中会忽略常数。

