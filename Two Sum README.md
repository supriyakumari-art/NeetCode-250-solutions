# Two Sum – LeetCode 1

**NeetCode 250 | Arrays & Hashing | Easy**

## Problem Statement

Given an array of integers `nums` and an integer `target`, return the indices of the two numbers such that they add up to the target.

You may assume that each input has exactly one solution, and you cannot use the same element twice.

## Example

**Input:**
```python
nums = [2, 7, 11, 15]
target = 9
```

**Output:**
```python
[0, 1]
```

**Explanation:**

Because `nums[0] + nums[1] == 9`.

## Approach: Hash Map

1. Create an empty dictionary called `hashmap`.
2. Iterate through the array using `enumerate()`.
3. Calculate the complement using `target - num`.
4. Check whether the complement exists in the dictionary.
5. If it exists, return the complement's index and the current index.
6. Otherwise, store the current number and its index in the dictionary.

## Complexity Analysis

- **Time Complexity:** O(N) – We traverse the array once, and dictionary lookups take O(1) average time.
- **Space Complexity:** O(N) – The dictionary may store up to N elements.

## Concepts Used

- Array
- Hash Map
- Dictionary
- Complement Technique

## Problem Details

- **LeetCode:** 1 – Two Sum
- **Difficulty:** Easy
- **NeetCode Roadmap:** NeetCode 250
- **Category:** Arrays & Hashing
