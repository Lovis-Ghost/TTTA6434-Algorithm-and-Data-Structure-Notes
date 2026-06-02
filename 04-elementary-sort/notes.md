# Chapter 4: Elementary Sort

# 第 4 章：基础排序

## 1. Key Idea / 核心思想

**English:**

Elementary sorting algorithms arrange data in order using simple comparison and movement steps.

**中文：**

基础排序算法通过比较和移动元素，把数据整理成指定顺序。

## 2. Key Concepts / 关键概念

**English:**

- Bubble sort compares neighboring elements.
- Selection sort selects the smallest or largest element.
- Insertion sort inserts each element into the correct position.
- These algorithms are easy to understand but usually slow for large data.

**中文：**

- 冒泡排序比较相邻元素。
- 选择排序每次选择最小或最大的元素。
- 插入排序把每个元素插入到正确位置。
- 这些算法容易理解，但处理大量数据时通常较慢。

## 3. Step-by-step Explanation / 分步骤理解

**English:**

1. Start with an unsorted list.
2. Compare elements.
3. Swap or move elements if needed.
4. Repeat until the list is sorted.

**中文：**

1. 从一个未排序的列表开始。
2. 比较元素。
3. 如果需要，就交换或移动元素。
4. 重复直到列表有序。

## 4. Simple Example / 简单例子

**English:**

```python
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(0, len(items) - i - 1):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
    return items
```

**中文：**

这个例子是冒泡排序。它不断比较相邻元素，如果顺序不对就交换。

## 5. My Understanding / 我的理解

**English:**

I can understand elementary sorting by drawing the list and showing each swap.

**中文：**

我可以通过画出列表并标出每次交换来理解基础排序。

## 6. Common Exam Points / 常见考点

**English:**

- Explain bubble sort, selection sort, and insertion sort.
- Trace sorting steps by hand.
- Know that many elementary sorts have `O(n^2)` time complexity.

**中文：**

- 解释冒泡、选择和插入排序。
- 手动追踪排序步骤。
- 记住很多基础排序的时间复杂度是 `O(n^2)`。

