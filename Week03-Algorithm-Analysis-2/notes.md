# Week 03: Algorithm Analysis 2

## Topic Overview

This week continues algorithm analysis with more examples and common complexity patterns.

## Key Concepts

- Best case, average case, and worst case may be different.
- Nested loops often increase time complexity.
- Logarithmic time usually appears when the problem size is reduced by half.
- Recursive algorithms need careful analysis.

## Step-by-step Explanation

1. Identify whether the algorithm has loops, nested loops, or recursion.
2. Decide how the input size changes during execution.
3. Find the dominant part of the algorithm.
4. Write the complexity using the simplest Big O form.

## Time Complexity / Space Complexity

- Binary search has time complexity `O(log n)`.
- Two nested loops over the same list often give `O(n^2)`.
- Recursive algorithms may use extra stack space.

## Python Example

```python
def count_pairs(numbers):
    count = 0
    for i in range(len(numbers)):
        for j in range(i + 1, len(numbers)):
            count += 1
    return count

print(count_pairs([1, 2, 3, 4]))
```

## Practice Questions

1. What is the difference between best case and worst case?
2. Why is binary search `O(log n)`?
3. What is the complexity of two nested loops?

## My Reflection

This topic is more challenging because different code patterns have different growth rates. I need more practice tracing loops and recursion.

