# Week 02: Algorithm Analysis 1

## Topic Overview

This week focuses on understanding how to measure the efficiency of an algorithm.

## Key Concepts

- An algorithm is a step-by-step method to solve a problem.
- Algorithm analysis helps compare different solutions.
- Time complexity estimates how running time grows.
- Space complexity estimates how memory usage grows.
- Big O notation describes the upper bound of growth.

## Step-by-step Explanation

1. Look at the main operations in the algorithm.
2. Count how many times the operations run.
3. Ignore small constants and less important terms.
4. Express the result using Big O notation.

## Time Complexity / Space Complexity

- `O(1)` means constant time.
- `O(n)` means the running time grows with the input size.
- `O(n^2)` often happens with nested loops.
- Space complexity can be `O(1)` if only a few extra variables are used.

## Python Example

```python
def find_max(numbers):
    largest = numbers[0]
    for number in numbers:
        if number > largest:
            largest = number
    return largest

print(find_max([4, 7, 1, 9, 2]))
```

## Practice Questions

1. What does Big O notation describe?
2. What is the time complexity of a single loop over a list?
3. Why do we ignore constants in Big O notation?

## My Reflection

I understood that Big O is not about exact running time. It is about how fast the algorithm grows when the input becomes bigger.

