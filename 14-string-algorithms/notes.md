# Chapter 14: String Algorithms

# 第 14 章：字符串算法

## 1. Key Idea / 核心思想

**English:**

String algorithms process text, such as searching for a pattern inside a string.

**中文：**

字符串算法用于处理文本，例如在字符串中查找某个模式。

## 2. Key Concepts / 关键概念

**English:**

- A string is a sequence of characters.
- Pattern matching means finding a smaller string inside a larger string.
- Placeholder: Add specific string algorithms covered in class.

**中文：**

- 字符串是一串字符。
- 模式匹配是在较长字符串中寻找较短字符串。
- 占位：之后补充课堂讲到的具体字符串算法。

## 3. Step-by-step Explanation / 分步骤理解

**English:**

1. Read the text and pattern.
2. Compare characters carefully.
3. Move through the text.
4. Return the matching position or report no match.

**中文：**

1. 读取文本和模式。
2. 仔细比较字符。
3. 在文本中移动检查位置。
4. 返回匹配位置，或说明没有匹配。

## 4. Simple Example / 简单例子

**English:**

```python
def simple_search(text, pattern):
    for i in range(len(text) - len(pattern) + 1):
        if text[i:i + len(pattern)] == pattern:
            return i
    return -1
```

**中文：**

这个例子使用简单方法查找子字符串，找到就返回开始位置，找不到就返回 -1。

## 5. My Understanding / 我的理解

**English:**

Placeholder: I will update this after learning the string algorithms in more detail.

**中文：**

占位：学习更多字符串算法后，我会补充自己的理解。

## 6. Common Exam Points / 常见考点

**English:**

- Explain what a string is.
- Explain pattern matching.
- Trace a simple string search.
- Add specific algorithm points after class.

**中文：**

- 解释什么是字符串。
- 解释什么是模式匹配。
- 手动追踪简单字符串查找。
- 课后补充具体算法考点。

