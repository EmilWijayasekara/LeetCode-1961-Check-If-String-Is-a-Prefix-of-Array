# LeetCode Practice  (Day 24)


## About the problem
- *Problem Number* : 1961
- *Problem Name* :  [Check If String Is a Prefix of Array](https://leetcode.com/problems/check-if-string-is-a-prefix-of-array/description/ "https://leetcode.com/problems/check-if-string-is-a-prefix-of-array/description/")
- *Problem difficulty* : Easy 🟢
- *Programming language used* - Java

## Problem

Given a string  `s`  and an array of strings  `words`, determine whether  `s`  is a  **prefix string**  of  `words`.

A string  `s`  is a  **prefix string**  of  `words`  if  `s`  can be made by concatenating the first  `k`  strings in  `words`  for some  **positive**  `k`  no larger than  `words.length`.

Return  `true` _if_ `s` _is a  **prefix string**  of_ `words`_, or_ `false` _otherwise_.

**Example 1:**

```
Input: s = "iloveleetcode", words = ["i","love","leetcode","apples"]
Output: true
Explanation:
s can be made by concatenating "i", "love", and "leetcode" together.
```

**Example 2:**

```
Input: s = "iloveleetcode", words = ["apples","i","love","leetcode"]
Output: false
Explanation:
It is impossible to make s using a prefix of arr.
```

**Constraints:**

-   `1 <= words.length <= 100`
-   `1 <= words[i].length <= 20`
-   `1 <= s.length <= 1000`
-   `words[i]`  and  `s`  consist of only lowercase English letters.

## Approach Explanation

By iteratively checking if the concatenation of the first k strings in the 'words' array matches the given string 's'. I used a loop to build a cumulative string, checking at each step if it matches 's'. If a match is found, I return true; otherwise, I continue the loop. If 's' is not a prefix string of 'words', or its length is less than the length of the first string in 'words', I return false. My approach is straightforward, focusing on building and comparing strings incrementally to determine if 's' can be formed by concatenating a prefix of 'words'. It offers a clear and effective way to solve the problem while handling the given constraints.

### If you have suggestions for improvement or would like to contribute to this solution, feel free to create a pull request. 🙌😇
