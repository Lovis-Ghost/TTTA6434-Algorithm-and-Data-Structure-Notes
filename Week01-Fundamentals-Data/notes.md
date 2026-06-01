# Week 01: Fundamentals of Data

## Topic Overview

This week introduces the basic idea of data, data types, and how data can be stored and processed in a program.

## Key Concepts

- Data is information used by a program.
- A data type tells the computer what kind of value is stored.
- Common data types include integers, floats, strings, booleans, lists, tuples, sets, and dictionaries.
- A data structure is a way to organize data so it can be used efficiently.

## Step-by-step Explanation

1. Identify the type of data needed for a problem.
2. Choose a suitable data structure.
3. Store the data in the program.
4. Access, update, or delete the data when needed.
5. Think about whether the chosen structure is efficient.

## Time Complexity / Space Complexity

- Accessing an item in a Python list by index is usually `O(1)`.
- Searching through an unsorted list is usually `O(n)`.
- Space complexity depends on how many values are stored.

## Python Example

```python
student = {
    "name": "Ali",
    "course": "TTTA6434",
    "marks": [80, 75, 90]
}

average = sum(student["marks"]) / len(student["marks"])
print(student["name"], average)
```

## Practice Questions

1. What is the difference between data and a data structure?
2. When should we use a list instead of a dictionary?
3. Give one example of structured data from daily life.

## My Reflection

I learned that choosing the correct way to store data is important before solving a problem. I still need to practice deciding which data structure is best for different situations.

