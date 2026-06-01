# Week 04: Elementary Sort

## Topic Overview

This week introduces simple sorting algorithms such as bubble sort, selection sort, and insertion sort.

## Key Concepts

- Sorting arranges data in a specific order.
- Elementary sorting algorithms are easy to understand but not always efficient.
- Bubble sort compares neighboring items.
- Selection sort repeatedly selects the smallest item.
- Insertion sort builds a sorted part one item at a time.

## Step-by-step Explanation

1. Start with an unsorted list.
2. Compare items based on the sorting rule.
3. Swap or move items when needed.
4. Repeat until the list is sorted.

## Time Complexity / Space Complexity

- Bubble sort: `O(n^2)` time, `O(1)` extra space.
- Selection sort: `O(n^2)` time, `O(1)` extra space.
- Insertion sort: `O(n^2)` worst case, `O(1)` extra space.

## Python Example

```python
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(0, len(items) - i - 1):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
    return items

print(bubble_sort([5, 2, 4, 1, 3]))
```

## Practice Questions

1. How does bubble sort work?
2. Which elementary sort is usually better for nearly sorted data?
3. Why are elementary sorts slow for large data?

## My Reflection

I can follow elementary sorting because the steps are visual. The main thing I need to remember is why the time complexity becomes `O(n^2)`.

