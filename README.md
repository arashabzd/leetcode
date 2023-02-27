# LeetCode
LeetCode Practice

Problem | Difficulty | Tags | Notes
---|---|---|---
[TwoSum](https://leetcode.com/problems/two-sum/description/) | Easy | `Array` `Hash Table` `Two Pointers` | **Brute Force** $\mathcal O(n^2)$ <br/><br/> **Two Pointers** $\mathcal O(n\log n)$: *Sort and set two pointer at left and right of the list, increase left if `sum < target` and decrease right if `sum > target`.* <br/><br/> **Two-pass Hash Table** $\mathcal O(n)$: *Build a {number: index} table, for each element look for `target - element` in the table.* <br/><br/> **One-pass Hash Table** $\mathcal O(n)$: *Sreate the table on the fly.*
[ThreeSum](https://leetcode.com/problems/3sum/) | Medium | `Array` `Hash Table` `Two Pointers` | **Two Pointers** $\mathcal O (n^2)$: *Sort and iterate the list for target, use two poiters approach to search in the rest of the list.* <br/><br/> **Hash Table** $\mathcal O (n^2)$: *Sort and build a {number: index} table, iterate the list for two numbers and search the third number in the table.*
[ThreeSum Closest](https://leetcode.com/problems/3sum-closest/) | Medium | `Array` `Two Pointers` | **Two Pointers** $\mathcal O (n^2)$: Same as Two Pointers solution for ThreeSum problem but keep track of best distance and best sum.
[Longest Common Prefix](https://leetcode.com/problems/longest-common-prefix/description/) | Easy | `String` | **Horizontal** $\mathcal O (\#c)$: $lcp(s_1, s_2, s_3) = lcp(lcp(s_1, s_2), s_3)$ <br/><br/> **Vertical** $\mathcal O (\#c)$: Find the shortest string and match its characters, one by one, with the rest of the strings.
[Longest Substring without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters/description/) | Medium | `String` `Window` `Hash Table` | **Window** $\mathcal O (n)$: Add unseen characters to a {char: index} table until you find a character that you have seen. If the seen character is outside of current window keep going else move the left pointer to the right of the previously seen character.

