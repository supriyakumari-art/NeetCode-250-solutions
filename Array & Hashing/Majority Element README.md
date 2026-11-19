# Majority Element

## Problem
Given an array `nums` of size `n`, return the majority element.

The majority element is the element that appears more than `n // 2` times.

## Approach: Sorting

1. Sort the array in ascending order.
2. The majority element will always be present at the middle index.
3. Return `nums[len(nums) // 2]`.

## Example

**Input:**
```python
nums = [3, 2, 3]
```

**Output:**
```python
3
```

## Complexity Analysis

- **Time Complexity:** O(n log n) – Sorting the array takes O(n log n) time.
- **Space Complexity:** O(1) auxiliary space – Sorting is done in place (depending on the sorting implementation).

## Topic
- Array
- Sorting
- NeetCode 250

## Language
Python 3
