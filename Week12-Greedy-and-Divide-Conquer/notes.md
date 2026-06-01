# Week 12: Greedy and Divide Conquer

## Topic Overview

This week covers two problem-solving strategies: greedy algorithms and divide and conquer.

## Key Concepts

- Greedy algorithms make the best local choice at each step.
- Divide and conquer splits a problem into smaller subproblems.
- Greedy is simple but does not always give the best final answer.
- Divide and conquer often uses recursion.

## Step-by-step Explanation

1. For greedy, choose the best option available now.
2. Repeat until the solution is complete.
3. For divide and conquer, divide the problem into smaller parts.
4. Solve the smaller parts.
5. Combine the results.

## Time Complexity / Space Complexity

- Greedy complexity depends on the number of choices and sorting if needed.
- Divide and conquer complexity often depends on the recurrence relation.
- Recursive divide and conquer may use extra stack space.

## Python Example

```python
def make_change(amount, coins):
    result = []
    for coin in sorted(coins, reverse=True):
        while amount >= coin:
            amount -= coin
            result.append(coin)
    return result

print(make_change(18, [10, 5, 1]))
```

## Practice Questions

1. What is a greedy choice?
2. Why does greedy not always produce the best answer?
3. What are the main steps of divide and conquer?

## My Reflection

I learned that strategy matters, not only coding. I need to understand the problem before deciding whether greedy or divide and conquer is suitable.

