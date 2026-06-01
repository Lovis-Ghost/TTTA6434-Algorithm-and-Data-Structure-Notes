# Week 06: Searching

## Topic Overview

This week introduces searching methods used to find an item in a collection.

## Key Concepts

- Linear search checks items one by one.
- Binary search works only when the data is sorted.
- Searching efficiency depends on how the data is organized.

## Step-by-step Explanation

1. Decide whether the data is sorted or unsorted.
2. Use linear search for simple unsorted data.
3. Use binary search for sorted data.
4. Compare the target value with the current item or middle item.
5. Stop when the value is found or when no possible position remains.

## Time Complexity / Space Complexity

- Linear search: `O(n)` time and `O(1)` space.
- Binary search: `O(log n)` time and `O(1)` space for iterative version.

## Python Example

```python
def binary_search(items, target):
    left = 0
    right = len(items) - 1

    while left <= right:
        mid = (left + right) // 2
        if items[mid] == target:
            return mid
        if items[mid] < target:
            left = mid + 1
        else:
            right = mid - 1

    return -1

print(binary_search([1, 3, 5, 7, 9], 7))
```

## Practice Questions

1. Why must binary search use sorted data?
2. What is the worst case for linear search?
3. Compare linear search and binary search.

## My Reflection

Binary search is efficient, but I need to be careful with the left, right, and middle indexes.

