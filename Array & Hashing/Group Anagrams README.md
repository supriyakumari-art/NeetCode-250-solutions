49. Group Anagrams
Platform: LeetCode
Problem: Group Anagrams
NeetCode: NeetCode 250
Difficulty: Medium
Topics: Array, Hash Table, String, Sorting
Language: Python
Approach: Hash Map + Sorting
Problem Description

Given an array of strings strs, group the anagrams together. You can return the answer in any order.

Anagrams are words that contain the same characters with the same frequency but in a different order.

Example

Input:

python
strs = ["eat", "tea", "tan", "ate", "nat", "bat"]


Output:

python
[["eat", "tea", "ate"], ["tan", "nat"], ["bat"]]

Approach: Hash Map + Sorting
Intuition

Two strings are anagrams if they contain exactly the same characters with the same frequency.

If we sort the characters of each word, all anagrams will produce the same sorted string.

For example:

Word	Sorted Key
eat	aet
tea	aet
ate	aet
tan	ant
nat	ant
bat	abt

We can use these sorted strings as dictionary keys to group anagrams together.

Algorithm
Create an empty dictionary called anagrams.
Iterate through each word in the input list.
Sort the characters of the current word and join them to create a key.
If the key does not exist in the dictionary, initialize it with an empty list.
Append the original word to the corresponding dictionary key.
Return all dictionary values as a list.

Complexity Analysis

Let:

n = Number of strings in the input.
k = Maximum length of a string.

Time Complexity: O(n × k log k)

We iterate through all n strings.
Sorting each string takes O(k log k) time.
Dictionary insertion and lookup take O(1) average time.

Therefore, total time complexity is:

O(n × k log k)

Space Complexity: O(n × k)

The dictionary stores the original strings in groups.
Sorted keys also require additional space.

Therefore, total space complexity is O(n × k).

Key Concepts Learned
Hash Maps / Dictionaries
Sorting Strings
Anagram Detection
Grouping Using Common Keys
String Manipulation
Important Takeaway

The key idea is to convert each string into a canonical representation by sorting its characters.

All anagrams share the same sorted representation, allowing us to group them efficiently using a hash map.

Alternative Optimization: A character-frequency array of size 26 can replace sorting and achieve O(n × k) time complexity when the input contains only lowercase English letters.

Status: Solved ✅
Approach: Hash Map + Sorting
Language: Python
