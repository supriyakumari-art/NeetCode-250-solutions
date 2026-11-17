# Concatenation of Array – LeetCode 1929

**NeetCode 250 | Arrays & Hashing | Easy**

## Problem Statement
Given an integer array `nums` of length `n`, create an array `ans` of length `2n` where `ans` consists of two copies of `nums` concatenated together.

## Approach: Nested Loop

1. Create an empty list `ans`.
2. Use an outer loop to repeat the process twice.
3. Use an inner loop to iterate through every element in `nums`.
4. Append each element to `ans`.
5. Return the final array.

## Example

**Input:**
```python
nums = [1, 2, 1]
```

**Output:**
```python
[1, 2, 1, 1, 2, 1]
```

**Explanation:**

The original array `[1, 2, 1]` is repeated twice.

## Complexity Analysis

- **Time Complexity:** O(N), where N is the length of the input array.
- **Space Complexity:** O(N), for the resulting array of size 2N.

## Concepts Used
- Array
- Nested Loops
- List Operations

## Alternative Python Solution

```python
class Solution:
    def getConcatenation(self, nums: List[int]) -> List[int]:
        return nums * 2
```

## Problem Details
- **LeetCode:** 1929 – Concatenation of Array
- **Difficulty:** Easy
- **NeetCode Roadmap:** NeetCode 250
- **Category:** Arrays & Hashing
