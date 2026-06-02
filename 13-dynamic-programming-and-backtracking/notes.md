# Chapter 13: Dynamic Programming and Backtracking

# 第 13 章：动态规划与回溯

## 1. Key Idea / 核心思想

**English:**

Dynamic programming stores answers to subproblems. Backtracking explores choices and goes back when a choice does not work.

**中文：**

动态规划会存储子问题答案。回溯会尝试选择，如果选择不合适就退回。

## 2. Key Concepts / 关键概念

**English:**

- Dynamic programming avoids repeated work.
- Memoization uses recursion with caching.
- Tabulation uses a table.
- Backtracking is useful for search and combination problems.

**中文：**

- 动态规划避免重复计算。
- 记忆化是递归加缓存。
- 表格法使用表来保存结果。
- 回溯常用于搜索和组合问题。

## 3. Step-by-step Explanation / 分步骤理解

**English:**

1. For dynamic programming, find repeated subproblems.
2. Store subproblem answers.
3. Build the final answer.
4. For backtracking, choose one option.
5. Continue or undo the choice if it fails.

**中文：**

1. 动态规划先找重复子问题。
2. 保存子问题答案。
3. 构造最终答案。
4. 回溯先选择一个选项。
5. 如果失败，就撤销选择并尝试其他选项。

## 4. Simple Example / 简单例子

**English:**

```python
def fibonacci(n, memo=None):
    if memo is None:
        memo = {}
    if n in memo:
        return memo[n]
    if n <= 1:
        return n
    memo[n] = fibonacci(n - 1, memo) + fibonacci(n - 2, memo)
    return memo[n]
```

**中文：**

这个例子使用记忆化保存 Fibonacci 的中间结果，避免重复计算。

## 5. My Understanding / 我的理解

**English:**

Dynamic programming is hard at first because I need to find the repeated subproblems.

**中文：**

动态规划一开始比较难，因为我需要先找出重复子问题。

## 6. Common Exam Points / 常见考点

**English:**

- Explain memoization and tabulation.
- Identify repeated subproblems.
- Explain backtracking choice and undo steps.

**中文：**

- 解释记忆化和表格法。
- 找出重复子问题。
- 解释回溯中的选择和撤销步骤。

