# Chapter 12: Greedy and Divide and Conquer

# 第 12 章：贪心与分治

## 1. Key Idea / 核心思想

**English:**

Greedy and divide and conquer are two common algorithm design strategies.

**中文：**

贪心和分治是两种常见的算法设计策略。

## 2. Key Concepts / 关键概念

**English:**

- Greedy chooses the best local option at each step.
- Greedy is simple but not always correct for every problem.
- Divide and conquer splits a problem into smaller subproblems.
- Recursion is often used in divide and conquer.

**中文：**

- 贪心每一步选择当前看起来最好的选项。
- 贪心简单，但不是每个问题都能得到正确最优解。
- 分治把大问题拆成小问题。
- 分治经常使用递归。

## 3. Step-by-step Explanation / 分步骤理解

**English:**

1. For greedy, make a local best choice.
2. Repeat until the solution is complete.
3. For divide and conquer, divide the problem.
4. Solve smaller parts.
5. Combine the answers.

**中文：**

1. 贪心先选择当前局部最优。
2. 重复直到得到完整解。
3. 分治先拆分问题。
4. 解决小问题。
5. 合并答案。

## 4. Simple Example / 简单例子

**English:**

```python
def make_change(amount, coins):
    result = []
    for coin in sorted(coins, reverse=True):
        while amount >= coin:
            amount -= coin
            result.append(coin)
    return result
```

**中文：**

这个例子用贪心思想找零钱，每次先选择面值最大的硬币。

## 5. My Understanding / 我的理解

**English:**

I need to check whether a greedy choice is really safe before using it.

**中文：**

使用贪心前，我需要判断当前最优选择是否真的能得到整体最优。

## 6. Common Exam Points / 常见考点

**English:**

- Explain greedy choice.
- Explain divide, solve, and combine.
- Know examples of greedy and divide and conquer algorithms.

**中文：**

- 解释贪心选择。
- 解释分解、解决和合并。
- 记住贪心和分治算法的例子。

