# Week 14: String Algorithms

## Topic Overview

This week is reserved for string processing and string algorithms.

## Key Concepts

- Strings are sequences of characters.
- String algorithms can search, compare, or match text.
- Placeholder: Add specific algorithms covered in class, such as pattern matching.

## Step-by-step Explanation

1. Read the input string.
2. Decide what pattern or condition is needed.
3. Compare characters carefully.
4. Return the position, count, or matched result.

## Time Complexity / Space Complexity

- Simple substring search can be `O(nm)` where `n` is text length and `m` is pattern length.
- Placeholder: Add complexity for the specific string algorithm covered.

## Python Example

```python
def simple_search(text, pattern):
    for i in range(len(text) - len(pattern) + 1):
        if text[i:i + len(pattern)] == pattern:
            return i
    return -1

print(simple_search("algorithm", "go"))
```

## Practice Questions

1. What is a string?
2. What does pattern matching mean?
3. Placeholder: What string algorithm was covered this week?

## My Reflection

Placeholder: I will update this after learning the string algorithms in more detail.

