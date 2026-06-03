# Chapter 2: Algorithm Analysis I

# 第二章：算法分析 I

## 1. Key Idea / 核心思想

**English:**

Algorithm analysis is used to estimate how much time and memory an algorithm needs. It helps us compare different algorithms and judge whether an algorithm is efficient or not.

Usually, we mainly look at:

- Time complexity
- Space complexity

**中文：**

算法分析是用来估计一个算法需要多少运行时间和内存空间。它可以帮助我们比较不同算法，判断一个算法好不好、效率高不高。

通常我们主要分析：

- 时间复杂度
- 空间复杂度

## 2. Why Not Use Actual Running Time? / 为什么不能只看实际运行秒数？

**English:**

We should not only use actual running seconds because the result can be affected by many things, such as:

- Computer speed
- Programming language
- Compiler or interpreter
- Input data
- Running environment

For example, the same algorithm may run faster on a better computer. So actual seconds are not always fair for comparing algorithms.

Algorithm analysis focuses on how the running time grows when the input size becomes larger.

**中文：**

我们不能只看实际运行了几秒，因为运行时间会受到很多因素影响，例如：

- 电脑速度
- 编程语言
- 编译器或解释器
- 输入数据
- 运行环境

例如，同一个算法在性能更好的电脑上可能会跑得更快。所以只用秒数来比较算法并不公平。

算法分析更关注的是：当输入规模变大时，算法的运行时间怎样增长。

## 3. Input Size n / 输入规模 n

**English:**

Input size `n` means a measure of how large the input data is. Different problems may define `n` in different ways.

Examples:

- Sorting: `n` is the number of elements to be sorted.
- Searching: `n` is the number of elements in the search space.
- Matrix problem: `n` can mean the size or order of the matrix, or the total number of elements.

**中文：**

输入规模 `n` 表示输入数据有多大。不同问题中，`n` 的意思可能不同。

例子：

- 排序：`n` 是需要排序的元素数量。
- 查找：`n` 是查找范围中的元素数量。
- 矩阵问题：`n` 可以表示矩阵的大小、阶数，或者矩阵中的元素总数。

## 4. Time Complexity and Space Complexity / 时间复杂度与空间复杂度

**English:**

Time complexity describes how the time used by an algorithm grows when the input size grows.

Space complexity describes how the extra memory used by an algorithm grows when the input size grows.

They do not usually tell us the exact number of seconds or exact memory size. They describe the growth trend.

**中文：**

时间复杂度描述的是：当输入规模变大时，算法所需时间怎样增长。

空间复杂度描述的是：当输入规模变大时，算法额外使用的内存怎样增长。

它们通常不是精确说明几秒钟或多少 MB，而是描述增长趋势。

## 5. Basic Operations / 基本操作

**English:**

Basic operations are not high-level operations like searching, insertion, and deletion.

Basic operations usually mean primitive operations that take constant time, such as:

- Assignment
- Arithmetic operation
- Comparison
- Array indexing
- Reading or writing a value
- Return statement

When analyzing an algorithm, we often count how many times the important basic operation is executed.

**中文：**

基本操作不是像查找、插入、删除这种高层操作。

基本操作通常指的是花费常数时间的原始操作，例如：

- 赋值
- 算术运算
- 比较
- 数组下标访问
- 读取或写入一个值
- return 语句

分析算法时，我们常常会计算某个重要基本操作大概执行了多少次。

## 6. Best, Average, and Worst Case / 最好、平均、最坏情况

**English:**

- Best case means the algorithm runs in the best possible situation.
- Average case means the algorithm runs in a normal or expected situation.
- Worst case means the algorithm runs in the worst possible situation.

We usually focus on the worst case because it gives an upper bound. It tells us the maximum growth we need to prepare for, so it gives a guarantee.

**中文：**

- 最好情况表示算法在最理想情况下运行。
- 平均情况表示算法在一般或期望情况下运行。
- 最坏情况表示算法在最不理想情况下运行。

我们通常关注最坏情况，因为它给出一个上界。它告诉我们最多可能需要多少时间或资源，所以比较有保证。

## 7. Big-O Notation / Big-O 表示法

**English:**

Big-O notation describes the upper bound of the growth rate of an algorithm. It shows how fast the time or space requirement grows when `n` becomes larger.

Common Big-O examples:

- `O(1)`: constant
- `O(log n)`: logarithmic
- `O(n)`: linear
- `O(n log n)`: linearithmic
- `O(n^2)`: quadratic
- `O(2^n)`: exponential

Growth order:

```text
O(1) < O(log n) < O(n) < O(n log n) < O(n^2) < O(2^n)
```

**中文：**

Big-O 表示法用来描述算法增长率的上界。它表示当 `n` 变大时，时间或空间需求增长得有多快。

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

This loop runs `n` times, so the time complexity is `O(n)`.

Example 2:

```python
for i in range(n):
    for j in range(n):
        print(i, j)
```

The outer loop runs `n` times. For each outer loop, the inner loop also runs `n` times.

Total number of iterations is:

```text
n * n = n^2
```

So the time complexity is `O(n^2)`.

**中文：**

例子 1：

```python
for i in range(n):
    print(i)
```

这个循环执行 `n` 次，所以时间复杂度是 `O(n)`。

例子 2：

```python
for i in range(n):
    for j in range(n):
        print(i, j)
```

外层循环执行 `n` 次。每执行一次外层循环，内层循环也执行 `n` 次。

总执行次数是：

```text
n * n = n^2
```

所以时间复杂度是 `O(n^2)`。

## 9. My Understanding / 我的理解

**English:**

I understand that algorithm analysis is not about measuring exact seconds, but about understanding how the algorithm grows when the input becomes larger. The most important part for me is learning to recognize loops, nested loops, and common Big-O growth rates.

**中文：**

我理解算法分析不是为了测量精确的秒数，而是为了理解当输入变大时，算法会怎样增长。对我来说，最重要的是学会判断循环、嵌套循环，以及常见的 Big-O 增长率。

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
3. 解释为什么实际运行时间不够用。
4. 举出基本操作的例子。
5. 区分最好情况、平均情况和最坏情况。
6. 分析简单循环和嵌套循环。
