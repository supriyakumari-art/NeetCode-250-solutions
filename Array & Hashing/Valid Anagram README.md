# Valid Anagram

**NeetCode 150 – Array & Hashing**

## Problem
Given two strings `s` and `t`, determine whether `t` is an anagram of `s`.

Two strings are anagrams if they contain the same characters with the same frequency, but possibly in a different order.

## Approach: Sorting

1. Use Python's `sorted()` function to sort both strings.
2. Compare the sorted strings.
3. If both sorted strings are equal, return `True`.
4. Otherwise, return `False`.

## Example

**Input:**
```python
s = "anagram"
t = "nagaram"
```

**Output:**
```python
True
```

**Explanation:**

Both strings contain the same characters with the same frequency.

## Complexity Analysis

- **Time Complexity:** O(n log n) – Sorting both strings takes O(n log n) time.
- **Space Complexity:** O(n) – The sorted strings require additional space.

## Concepts Used
- Strings
- Sorting
- Comparison

## Difficulty
Easy

## Language
Python 3
