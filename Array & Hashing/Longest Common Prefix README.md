14. Longest Common Prefix
Platform: LeetCode
Problem: Longest Common Prefix
NeetCode: NeetCode 250
Difficulty: Easy
Topics: Array, String, Trie
Language: Python
Approach: Horizontal Scanning
Problem Description

Write a function to find the longest common prefix string amongst an array of strings.

If there is no common prefix, return an empty string "".

Example 1

Input:

python
strs = ["flower", "flow", "flight"]


Output:

python
"fl"

Example 2

Input:

python
strs = ["dog", "racecar", "car"]


Output:

python
""


Explanation: There is no common prefix among the input strings.

Approach: Horizontal Scanning
Intuition

The idea is to take the first string as the initial prefix and compare it with every other string.

If the current string does not start with the prefix, keep removing the last character from the prefix until a match is found.

Continue this process for all strings.

If the prefix becomes empty, return "" because no common prefix exists.

Algorithm
Check whether the input list is empty. If yes, return "".
Initialize prefix with the first string.
Iterate through the remaining strings.
Check whether each string starts with the current prefix using startswith().
If it does not match, remove the last character from the prefix.
Repeat until a common prefix is found.
If the prefix becomes empty, return "".
Return the final common prefix.

Dry Run

Input:

python
strs = ["flower", "flow", "flight"]

Step	Current String	Prefix	Action
1	flower	flower	Initial prefix
2	flow	flow	Remove characters until match
3	flight	fl	Remove characters until match

Output:

python
"fl"

Complexity Analysis

Let:

n = Number of strings.
m = Length of the longest string.

Time Complexity: O(n × m²)

We iterate through the strings.
In the worst case, the prefix can be shortened multiple times.
String slicing and startswith() can take O(m) time.

Therefore, the conservative worst-case time complexity for this implementation is O(n × m²).

Space Complexity: O(m)

The prefix variable stores a string of at most m characters.
String slicing creates temporary strings.
Key Concepts Learned
String Manipulation
Array Traversal
Prefix Matching
Horizontal Scanning
Python startswith() Method
String Slicing
Important Takeaway

The main idea is to use the first string as the initial prefix and continuously reduce it until it becomes a prefix of every string.

This approach is simple and effective for finding the longest common prefix.

Status: Solved ✅
Approach: Horizontal Scanning
Language: Python
