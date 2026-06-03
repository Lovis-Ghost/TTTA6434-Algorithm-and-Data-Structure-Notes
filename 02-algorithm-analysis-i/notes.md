# Chapter 2: Algorithm Analysis I

# 第二章：算法分析 I

## 1. Key Idea / 核心思想

**English:**

Algorithm analysis is used to estimate how much time and memory an algorithm needs. It helps us compare different algorithms and judge whether an algorithm is efficient or not.

The two main resources we usually study are:

- Time complexity
- Space complexity

**中文：**

算法分析是用来估计一个算法需要多少运行时间和内存空间。它可以帮助我们比较不同算法，并判断一个算法好不好、效率高不高。

我们通常主要分析两个资源：

- 时间复杂度
- 空间复杂度

## 2. Why Not Use Actual Running Time? / 为什么不能只看实际运行秒数？

**English:**

We cannot judge an algorithm only by actual running seconds because the result may change in different situations. Actual running time can depend on:

- Machine or computer speed
- Programming language
- Compiler or interpreter
- Input data
- System environment

Algorithm analysis focuses on how the running time grows when the input size becomes larger. This is more useful than only measuring exact seconds.

**中文：**

我们不能只用实际运行秒数来判断算法，因为不同情况下秒数可能会改变。实际运行时间可能受到这些因素影响：

- 电脑或机器速度
- 编程语言
- 编译器或解释器
- 输入数据
- 系统环境

算法分析更关注当输入规模变大时，运行时间怎样增长。这比只看精确秒数更有意义。

## 3. Input Size n / 输入规模 n

**English:**

Input size `n` means a measure of how large the input data is. The meaning of `n` depends on the problem.

- Sorting: `n` is the number of elements to be sorted.
- Searching: `n` is the number of elements in the search space.
- Matrix problem: `n` can mean the matrix size/order, or the total number of elements in the matrix.

**中文：**

输入规模 `n` 表示输入数据有多大。不同题目中，`n` 的意思可能不同。

- 排序：`n` 是要排序的元素数量。
- 搜索：`n` 是搜索范围中的元素数量。
- 矩阵问题：`n` 可以表示矩阵的阶数或大小，也可以表示矩阵中的元素总数。

## 4. Time Complexity and Space Complexity / 时间复杂度与空间复杂度

**English:**

Time complexity describes how the time used by an algorithm grows when the input size grows. It does not usually mean exact seconds. It describes the growth pattern.

Space complexity describes how the extra memory used by an algorithm grows when the input size grows. Extra memory may include arrays, temporary variables, recursion stack, or other storage used during the algorithm.

**中文：**

时间复杂度描述当输入规模变大时，算法所需时间如何增长。它通常不是指精确秒数，而是描述增长趋势。

空间复杂度描述当输入规模变大时，算法额外使用的内存如何增长。额外内存可能包括数组、临时变量、递归调用栈，或算法运行过程中使用的其他存储空间。

## 5. Basic Operations / 基本操作

**English:**

Basic operations are not high-level operations such as searching, insertion, or deletion. Those are usually complete algorithm tasks or data structure operations.

In algorithm analysis, basic operations usually mean primitive operations that take constant time.

Examples:

- Assignment
- Arithmetic operation
- Comparison
- Array indexing
- Reading or writing a value
- Return statement

**中文：**

基本操作不是指搜索、插入、删除这种比较高层的操作。那些通常是完整的算法任务，或者是数据结构中的操作。

在算法分析中，基本操作通常是指需要常数时间完成的原始操作。

例子：

- 赋值
- 算术运算
- 比较
- 数组下标访问
- 读取或写入一个值
- return 语句

## 6. Best, Average, and Worst Case / 最好、平均、最坏情况

**English:**

- Best case means the algorithm runs in the most favorable situation.
- Average case means the algorithm runs under normal or expected input situations.
- Worst case means the algorithm runs in the most unfavorable situation.

We usually focus on the worst case because it gives an upper bound. It tells us the maximum amount of work the algorithm may need, so it gives a guarantee even when the input is bad.

**中文：**

- 最好情况表示算法在最有利的输入情况下运行。
- 平均情况表示算法在一般或期望的输入情况下运行。
- 最坏情况表示算法在最不利的输入情况下运行。

我们通常关注最坏情况，因为它给出一个上界。它告诉我们算法最多可能需要做多少工作，所以即使输入很差，也能给我们一个保证。

## 7. Big-O Notation / Big-O 表示法

**English:**

Big-O notation describes the upper bound of the growth rate of an algorithm. It tells us how fast the time or memory usage grows when `n` becomes larger.

Common Big-O examples:

- `O(1)`: constant growth
- `O(log n)`: logarithmic growth
- `O(n)`: linear growth
- `O(n log n)`: linearithmic growth
- `O(n^2)`: quadratic growth
- `O(2^n)`: exponential growth

Growth order:

```text
O(1) < O(log n) < O(n) < O(n log n) < O(n^2) < O(2^n)
```

**中文：**

Big-O 表示法用来描述算法增长率的上界。它告诉我们当 `n` 变大时，时间或内存使用量增长得有多快。

常见 Big-O 例子：

- `O(1)`：常数增长
- `O(log n)`：对数增长
- `O(n)`：线性增长
- `O(n log n)`：线性对数增长
- `O(n^2)`：平方增长
- `O(2^n)`：指数增长

增长顺序：

```text
O(1) < O(log n) < O(n) < O(n log n) < O(n^2) < O(2^n)
```

## 8. Simple Code Examples / 简单代码例子

**English:**

Example 1:

```python
for i in range(n):
    print(i)
```

This loop runs `n` times. Each time it does a simple operation, so the time complexity is `O(n)`.

Example 2:

```python
for i in range(n):
    for j in range(n):
        print(i, j)
```

The outer loop runs `n` times, and for each outer loop, the inner loop also runs `n` times. The total number of iterations is `n * n`, so the time complexity is `O(n^2)`.

**中文：**

例子 1：

```python
for i in range(n):
    print(i)
```

这个循环执行 `n` 次。每次执行的是简单操作，所以时间复杂度是 `O(n)`。

例子 2：

```python
for i in range(n):
    for j in range(n):
        print(i, j)
```

外层循环执行 `n` 次，每一次外层循环中，内层循环也执行 `n` 次。总执行次数是 `n * n`，所以时间复杂度是 `O(n^2)`。

## 9. My Understanding / 我的理解

**English:**

I understand that algorithm analysis is not about measuring exact seconds, but about understanding how the algorithm grows when the input becomes larger. The most important part for me is learning to recognize loops, nested loops, and common Big-O growth rates.

**中文：**

我理解算法分析不是为了测量精确的运行秒数，而是为了理解当输入规模变大时，算法会怎样增长。对我来说，最重要的是学会判断循环、嵌套循环，以及常见的 Big-O 增长率。

## 10. Common Exam Points / 常见考点

**English:**

1. Define algorithm analysis.
2. Explain time complexity and space complexity.
3. Explain why actual running time is not enough.
4. Give examples of basic operations.
5. Differentiate best, average, and worst case.
6. Analyze simple loops and nested loops.

**中文：**

1. 定义什么是算法分析。
2. 解释时间复杂度和空间复杂度。
3. 解释为什么只看实际运行时间不够。
4. 举出基本操作的例子。
5. 区分最好情况、平均情况和最坏情况。
6. 分析简单循环和嵌套循环。
