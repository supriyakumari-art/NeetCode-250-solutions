# Contains Duplicate

**NeetCode 150 – Array & Hashing**

## Problem
Given an integer array `nums`, return `True` if any value appears at least twice in the array. Otherwise, return `False`.

## Approach: Brute Force

1. Use two nested loops to iterate through the array.
2. The outer loop selects an element.
3. The inner loop compares it with all the elements that come after it.
4. If two elements are equal, return `True`.
5. If no duplicate is found, return `False`.

## Example

**Input:**
```python
nums = [1, 2, 3, 1]
```

**Output:**
```python
True
```

**Explanation:**

The number `1` appears twice in the array, so the function returns `True`.

## Complexity Analysis

- **Time Complexity:** O(n²) – Two nested loops compare elements.
- **Space Complexity:** O(1) – No additional data structure is used.

## Concepts Used
- Arrays
- Nested Loops
- Brute Force Approach

## Difficulty
Easy

## Language
Python 3
