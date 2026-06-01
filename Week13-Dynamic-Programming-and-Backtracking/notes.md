# Week 13: Dynamic Programming and Backtracking

## Topic Overview

This week introduces dynamic programming and backtracking as strategies for solving more complex problems.

## Key Concepts

- Dynamic programming stores answers to subproblems to avoid repeated work.
- Memoization uses recursion with caching.
- Tabulation builds answers using a table.
- Backtracking tries choices and removes a choice if it does not work.

## Step-by-step Explanation

1. Identify repeated subproblems for dynamic programming.
2. Store answers in a cache or table.
3. Build the final answer from smaller answers.
4. For backtracking, choose one option.
5. Continue exploring or undo the choice when it fails.

## Time Complexity / Space Complexity

- Dynamic programming can reduce repeated recursion.
- Space complexity usually depends on the cache or table size.
- Backtracking can be expensive because it may explore many combinations.

## Python Example

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

print(fibonacci(10))
```

## Practice Questions

1. What is the purpose of memoization?
2. What is the difference between dynamic programming and backtracking?
3. Give one problem that can use dynamic programming.

## My Reflection

Dynamic programming feels difficult at first because I need to see the smaller subproblems. More practice will help me recognize the pattern.

