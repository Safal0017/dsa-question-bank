# Love Babbar DSA Cracker — Question Index

## Scope and provenance

This review draft follows the 448-entry, 15-section version of Love Babbar's DSA Cracker sheet, commonly called the “450 DSA sheet”. Counts include repeated entries and conceptual questions, not 448 distinct coding problems.

Question membership and order follow the [sheet mirror](https://github.com/dalpat98/DSA-Sheet-by-Love-Babbar). Cross-check navigation against [450 DSA](https://450dsa.com/) and its [linked-question dataset](https://github.com/AsishRaju/450-DSA/blob/c375f2df/src/450DSAFinal.js). Section-local IDs start at 1, whereas the tracker displays IDs starting at 0.

GFG articles often include solutions. To avoid spoilers, use the daily problem file first. A few sheet items are conceptual or originally hosted on SPOJ, HackerEarth, HackerRank or Google; these are labelled rather than silently replaced with unrelated LeetCode questions.

## Section navigation and counts

| Section | Entries |
| --- | ---: |
| [Arrays](#arrays) | 36 |
| [Matrix](#matrix) | 10 |
| [Strings](#strings) | 43 |
| [Searching and Sorting](#searching-and-sorting) | 36 |
| [Linked Lists](#linked-lists) | 36 |
| [Binary Trees](#binary-trees) | 35 |
| [Binary Search Trees](#binary-search-trees) | 22 |
| [Greedy](#greedy) | 35 |
| [Backtracking](#backtracking) | 19 |
| [Stacks and Queues](#stacks-and-queues) | 38 |
| [Heap](#heap) | 18 |
| [Graphs](#graphs) | 44 |
| [Trie](#trie) | 6 |
| [Dynamic Programming](#dynamic-programming) | 60 |
| [Bit Manipulation](#bit-manipulation) | 10 |
| Total | 448 |

## Arrays practice plan

| Plan | Arrays IDs | Ques Count |  
| ---  | ---------- |  ---: |    
| Day 1 | ARR-01–ARR-05 | 5 |  
| Day 2 | ARR-06–ARR-10 | 5 |  
| Day 3 | ARR-11–ARR-15 | 5 |  
| Day 4 | ARR-16–ARR-20 | 5 |  
| Day 5 | ARR-21–ARR-25 | 5 |  
| Day 6 | ARR-26–ARR-30 | 5 |  
| Day 7 | ARR-31–ARR-36 | 6 |  

## Important variant notes

- ARR-03 asks for both kth smallest and kth largest; its GFG destination judges only kth smallest. The Day 1 pack retains both parts and explains how to submit the GFG part.
- ARR-05 uses the linked GFG variant: non-negative numbers first, negative numbers last, retaining relative order within each group. The broad sheet title alone does not specify stability or which side.
- ARR-08 and ARR-13 both cover maximum-subarray sum. Both entries remain for count and order fidelity.
- ARR-25 is the general “more than n/k” problem. LeetCode Majority Element II fixes k = 3 and is not a full replacement.
- ARR-31 requires sum strictly greater than the threshold. LeetCode Minimum Size Subarray Sum uses greater than or equal, so it is not used as an exact substitute.
- ARR-34 is about merging adjacent array entries to make a palindrome, not swapping characters in a string. The similarly named LeetCode string problem is not equivalent.
- MAT-02 uses LeetCode Search a 2D Matrix. Its cross-row ordering assumption is stronger than simply having sorted rows and columns.
- SS-04 retains the sheet's “square root” wording. Some mirrors link to Count Squares instead; this index points to the square-root task.
- LL-25 retains the sheet's “rotate in groups” wording. Mirrors sometimes route it to group reversal; this remains a discovery link pending a precise variant choice.
- GP-34 and GP-35 repeat the water-jug task. Both are retained.
- A reused task in another section is not deduplicated; the sheet intentionally revisits several problems and techniques.

## Progress key

Check an entry only after you can explain your approach, implement it, validate examples and edge cases, and state its time and auxiliary-space complexity. No solution code or prescribed technique is included in this index.

## Arrays

36 entries.

- [ ] ARR-01 — [Reverse the array](https://www.geeksforgeeks.org/problems/reverse-an-array/1) — GFG practice
- [ ] ARR-02 — [Find the maximum and minimum element in an array](https://www.geeksforgeeks.org/problems/find-minimum-and-maximum-element-in-an-array4428/1) — GFG practice
- [ ] ARR-03 — [Find the kth maximum and minimum element of an array](https://www.geeksforgeeks.org/problems/kth-smallest-element5635/1) — GFG practice
- [ ] ARR-04 — [Sort an array of 0s, 1s and 2s without a general-purpose sorting algorithm](https://www.geeksforgeeks.org/problems/sort-an-array-of-0s-1s-and-2s4231/1) — GFG practice
- [ ] ARR-05 — [Move all negative elements to one side of the array](https://www.geeksforgeeks.org/problems/move-all-negative-elements-to-end1813/1) — GFG practice
- [ ] ARR-06 — [Find the union and intersection of two sorted arrays](https://www.geeksforgeeks.org/union-and-intersection-of-two-sorted-arrays-2/) — GFG article
- [ ] ARR-07 — [Cyclically rotate an array by one](https://www.geeksforgeeks.org/problems/cyclically-rotate-an-array-by-one/1) — GFG practice
- [ ] ARR-08 — [Find the largest-sum contiguous subarray](https://www.geeksforgeeks.org/problems/kadanes-algorithm/1) — GFG practice
- [ ] ARR-09 — [Minimise the maximum difference between heights](https://www.geeksforgeeks.org/problems/minimize-the-heights3351/1) — GFG practice
- [ ] ARR-10 — [Minimum jumps to reach the end of an array](https://www.geeksforgeeks.org/problems/minimum-number-of-jumps/1) — GFG practice
- [ ] ARR-11 — [Find the duplicate in an array of N+1 integers](https://leetcode.com/problems/find-the-duplicate-number/) — LeetCode
- [ ] ARR-12 — [Merge two sorted arrays without extra space](https://www.geeksforgeeks.org/problems/merge-two-sorted-arrays-1587115620/1) — GFG practice
- [ ] ARR-13 — [Kadane’s algorithm (retained repeated entry)](https://www.geeksforgeeks.org/problems/kadanes-algorithm/1) — GFG practice
- [ ] ARR-14 — [Merge intervals](https://leetcode.com/problems/merge-intervals/) — LeetCode
- [ ] ARR-15 — [Next permutation](https://leetcode.com/problems/next-permutation/) — LeetCode
- [ ] ARR-16 — [Count inversions](https://www.geeksforgeeks.org/problems/inversion-of-array/1) — GFG practice
- [ ] ARR-17 — [Best time to buy and sell stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock/) — LeetCode
- [ ] ARR-18 — [Count pairs with a given sum](https://www.geeksforgeeks.org/problems/count-pairs-with-given-sum5022/1) — GFG practice
- [ ] ARR-19 — [Common elements in three sorted arrays](https://www.geeksforgeeks.org/problems/common-elements1132/1) — GFG practice
- [ ] ARR-20 — [Rearrange alternating positive and negative items with O(1) extra space](https://www.geeksforgeeks.org/problems/array-of-alternate-ve-and-ve-nos1401/1) — GFG practice
- [ ] ARR-21 — [Check for a subarray with sum zero](https://www.geeksforgeeks.org/problems/subarray-with-0-sum/1) — GFG practice
- [ ] ARR-22 — [Factorial of a large number](https://www.geeksforgeeks.org/problems/factorials-of-large-numbers/1) — GFG practice
- [ ] ARR-23 — [Maximum-product subarray](https://www.geeksforgeeks.org/problems/maximum-product-subarray3604/1) — GFG practice
- [ ] ARR-24 — [Longest consecutive subsequence](https://www.geeksforgeeks.org/problems/longest-consecutive-subsequence/1) — GFG practice
- [ ] ARR-25 — [Find all elements appearing more than n/k times](https://www.geeksforgeeks.org/given-an-array-of-size-n-find-all-elements-that-appear-more-than-nk-times/) — GFG article
- [ ] ARR-26 — [Maximum stock profit with at most two transactions](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-iii/) — LeetCode
- [ ] ARR-27 — [Check whether an array is a subset of another](https://www.geeksforgeeks.org/problems/array-subset-of-another-array/1) — GFG practice
- [ ] ARR-28 — [Find a triplet with a given sum](https://www.geeksforgeeks.org/problems/triplet-sum-in-array/1) — GFG practice
- [ ] ARR-29 — [Trapping rain water](https://www.geeksforgeeks.org/problems/trapping-rain-water/1) — GFG practice
- [ ] ARR-30 — [Chocolate distribution problem](https://www.geeksforgeeks.org/problems/chocolate-distribution-problem/1) — GFG practice
- [ ] ARR-31 — [Smallest subarray with sum strictly greater than a given value](https://www.geeksforgeeks.org/problems/smallest-subarray-with-sum-greater-than-x/1) — GFG practice
- [ ] ARR-32 — [Three-way partitioning around a range](https://www.geeksforgeeks.org/problems/three-way-partitioning/1) — GFG practice
- [ ] ARR-33 — [Minimum swaps to bring elements <= k together](https://www.geeksforgeeks.org/problems/minimum-swaps-required-to-bring-all-elements-less-than-or-equal-to-k-together/1) — GFG practice
- [ ] ARR-34 — [Minimum merge operations to make an array palindrome](https://www.geeksforgeeks.org/find-minimum-number-of-merge-operations-to-make-an-array-palindrome/) — GFG article
- [ ] ARR-35 — [Median of two sorted arrays of equal size](https://www.geeksforgeeks.org/median-of-two-sorted-arrays/) — GFG article
- [ ] ARR-36 — [Median of two sorted arrays of different sizes](https://leetcode.com/problems/median-of-two-sorted-arrays/) — LeetCode

[Back to section counts](#section-navigation-and-counts)

## Matrix

10 entries.

- [ ] MAT-01 — [Spiral traversal of a matrix](https://www.geeksforgeeks.org/problems/spirally-traversing-a-matrix/1) — GFG practice
- [ ] MAT-02 — [Search an element in a matrix](https://leetcode.com/problems/search-a-2d-matrix/) — LeetCode
- [ ] MAT-03 — [Median in a row-wise sorted matrix](https://www.geeksforgeeks.org/problems/median-in-a-row-wise-sorted-matrix1527/1) — GFG practice
- [ ] MAT-04 — [Row with the maximum number of 1s](https://www.geeksforgeeks.org/problems/row-with-max-1s0023/1) — GFG practice
- [ ] MAT-05 — [Print a row-column sorted matrix in sorted order](https://www.geeksforgeeks.org/problems/sorted-matrix/1) — GFG practice
- [ ] MAT-06 — [Maximum-size rectangle of 1s](https://www.geeksforgeeks.org/problems/max-rectangle/1) — GFG practice
- [ ] MAT-07 — [Find a specific pair in a matrix](https://www.geeksforgeeks.org/find-a-specific-pair-in-matrix/) — GFG article
- [ ] MAT-08 — [Rotate a matrix by 90 degrees](https://www.geeksforgeeks.org/rotate-a-matrix-by-90-degree-in-clockwise-direction-without-using-any-extra-space/) — GFG article
- [ ] MAT-09 — [Kth smallest element in a row-column sorted matrix](https://www.geeksforgeeks.org/problems/kth-element-in-matrix/1) — GFG practice
- [ ] MAT-10 — [Common elements in all rows of a matrix](https://www.geeksforgeeks.org/common-elements-in-all-rows-of-a-given-matrix/) — GFG article

[Back to section counts](#section-navigation-and-counts)

## Strings

43 entries.

- [ ] STR-01 — [Reverse a string](https://leetcode.com/problems/reverse-string/) — LeetCode
- [ ] STR-02 — [Check whether a string is a palindrome](https://www.geeksforgeeks.org/problems/palindrome-string0817/1) — GFG practice
- [ ] STR-03 — [Find duplicate characters in a string](https://www.geeksforgeeks.org/print-all-the-duplicates-in-the-input-string/) — GFG article
- [ ] STR-04 — [Why are strings immutable in Java? (conceptual)](https://www.baeldung.com/java-string-immutable) — Conceptual reference (Baeldung)
- [ ] STR-05 — [Check whether one string is a rotation of another](https://www.geeksforgeeks.org/a-program-to-check-if-strings-are-rotations-of-each-other/) — GFG article
- [ ] STR-06 — [Check whether a string is a valid shuffle of two strings](https://leetcode.com/problems/interleaving-string/) — LeetCode
- [ ] STR-07 — [Count and say](https://leetcode.com/problems/count-and-say/) — LeetCode
- [ ] STR-08 — [Longest palindromic substring](https://www.geeksforgeeks.org/problems/longest-palindrome-in-a-string/1) — GFG practice
- [ ] STR-09 — [Longest repeating subsequence](https://www.geeksforgeeks.org/problems/longest-repeating-subsequence/1) — GFG practice
- [ ] STR-10 — [Print all subsequences of a string](https://www.geeksforgeeks.org/print-subsequences-string/) — GFG article
- [ ] STR-11 — [Print all permutations of a string](https://www.geeksforgeeks.org/problems/permutations-of-a-given-string2041/1) — GFG practice
- [ ] STR-12 — [Split a binary string into balanced substrings](https://www.geeksforgeeks.org/problems/split-the-binary-string-into-substrings-with-equal-number-of-0s-and-1s/1) — GFG practice
- [ ] STR-13 — [Word wrap](https://www.geeksforgeeks.org/problems/word-wrap1646/1) — GFG practice
- [ ] STR-14 — [Edit distance](https://www.geeksforgeeks.org/problems/edit-distance3702/1) — GFG practice
- [ ] STR-15 — [Next greater number with the same digits](https://www.geeksforgeeks.org/problems/next-permutation/1) — GFG practice
- [ ] STR-16 — [Balanced parentheses](https://www.geeksforgeeks.org/problems/parenthesis-checker2744/1) — GFG practice
- [ ] STR-17 — [Word break](https://www.geeksforgeeks.org/problems/word-break1352/1) — GFG practice
- [ ] STR-18 — [Rabin–Karp pattern searching](https://www.geeksforgeeks.org/rabin-karp-algorithm-for-pattern-searching/) — GFG article
- [ ] STR-19 — [KMP pattern searching](https://www.geeksforgeeks.org/kmp-algorithm-for-pattern-searching/) — GFG article
- [ ] STR-20 — [Convert a sentence to its mobile keypad sequence](https://www.geeksforgeeks.org/convert-sentence-equivalent-mobile-numeric-keypad-sequence/) — GFG article
- [ ] STR-21 — [Minimum bracket reversals to balance an expression](https://www.geeksforgeeks.org/problems/count-the-reversals0401/1) — GFG practice
- [ ] STR-22 — [Count all palindromic subsequences](https://www.geeksforgeeks.org/problems/count-palindromic-subsequences/1) — GFG practice
- [ ] STR-23 — [Count occurrences of a string in a 2D character array](https://www.geeksforgeeks.org/find-count-number-given-string-present-2d-character-array/) — GFG article
- [ ] STR-24 — [Search a word in a 2D grid](https://www.geeksforgeeks.org/problems/find-the-string-in-grid0111/1) — GFG practice
- [ ] STR-25 — [Boyer–Moore pattern searching](https://www.geeksforgeeks.org/boyer-moore-algorithm-for-pattern-searching/) — GFG article
- [ ] STR-26 — [Roman numeral to decimal](https://www.geeksforgeeks.org/problems/roman-number-to-integer3201/1) — GFG practice
- [ ] STR-27 — [Longest common prefix](https://leetcode.com/problems/longest-common-prefix/) — LeetCode
- [ ] STR-28 — [Minimum flips to make a binary string alternate](https://www.geeksforgeeks.org/problems/min-number-of-flips3210/1) — GFG practice
- [ ] STR-29 — [First repeated word in a string](https://www.geeksforgeeks.org/find-first-repeated-word-string/) — GFG article
- [ ] STR-30 — [Minimum swaps for bracket balancing](https://www.geeksforgeeks.org/problems/minimum-swaps-for-bracket-balancing2704/1) — GFG practice
- [ ] STR-31 — [Longest common subsequence of two strings](https://www.geeksforgeeks.org/problems/longest-common-subsequence-1587115620/1) — GFG practice
- [ ] STR-32 — [Generate all valid IP addresses](https://www.geeksforgeeks.org/program-generate-possible-valid-ip-addresses-given-string/) — GFG article
- [ ] STR-33 — [Smallest window containing every distinct character of the string](https://www.geeksforgeeks.org/problems/smallest-distant-window3132/1) — GFG practice
- [ ] STR-34 — [Rearrange characters so adjacent characters differ](https://www.geeksforgeeks.org/problems/rearrange-characters4649/1) — GFG practice
- [ ] STR-35 — [Minimum characters to add at the front to make a palindrome](https://www.geeksforgeeks.org/minimum-characters-added-front-make-string-palindrome/) — GFG article
- [ ] STR-36 — [Group anagrams together](https://leetcode.com/problems/group-anagrams/) — LeetCode
- [ ] STR-37 — [Smallest window containing all characters of another string](https://leetcode.com/problems/minimum-window-substring/) — LeetCode
- [ ] STR-38 — [Recursively remove all adjacent duplicates](https://www.geeksforgeeks.org/problems/recursively-remove-all-adjacent-duplicates0744/1) — GFG practice
- [ ] STR-39 — [Wildcard string matching](https://www.geeksforgeeks.org/problems/wildcard-string-matching1126/1) — GFG practice
- [ ] STR-40 — [Customers who could not get a computer](https://www.geeksforgeeks.org/function-to-find-number-of-customers-who-could-not-get-a-computer/) — GFG article
- [ ] STR-41 — [Transform one string to another using minimum given operations](https://www.geeksforgeeks.org/transform-one-string-to-another-using-minimum-number-of-given-operation/) — GFG article
- [ ] STR-42 — [Check whether two strings are isomorphic](https://www.geeksforgeeks.org/problems/isomorphic-strings-1587115620/1) — GFG practice
- [ ] STR-43 — [Print all sentences from a list of word lists](https://www.geeksforgeeks.org/recursively-print-all-sentences-that-can-be-formed-from-list-of-word-lists/) — GFG article

[Back to section counts](#section-navigation-and-counts)

## Searching and Sorting

36 entries.

- [ ] SS-01 — [First and last positions of an element in a sorted array](https://www.geeksforgeeks.org/problems/first-and-last-occurrences-of-x3116/1) — GFG practice
- [ ] SS-02 — [Find fixed points (value equals index)](https://www.geeksforgeeks.org/problems/value-equal-to-index-value1330/1) — GFG practice
- [ ] SS-03 — [Search in a rotated sorted array](https://leetcode.com/problems/search-in-rotated-sorted-array/) — LeetCode
- [ ] SS-04 — [Square root of an integer](https://leetcode.com/problems/sqrtx/) — LeetCode
- [ ] SS-05 — [Maximum and minimum using minimum comparisons](https://www.geeksforgeeks.org/maximum-and-minimum-in-an-array/) — GFG article
- [ ] SS-06 — [Optimum point location to minimise total distance](https://www.geeksforgeeks.org/optimum-location-point-minimize-total-distance/) — GFG article
- [ ] SS-07 — [Find the repeating and missing numbers](https://www.geeksforgeeks.org/problems/find-missing-and-repeating2512/1) — GFG practice
- [ ] SS-08 — [Majority element](https://www.geeksforgeeks.org/problems/majority-element-1587115620/1) — GFG practice
- [ ] SS-09 — [Search where adjacent elements differ by at most k](https://www.geeksforgeeks.org/problems/searching-in-an-array-where-adjacent-differ-by-at-most-k0456/1) — GFG practice
- [ ] SS-10 — [Find a pair with a given difference](https://www.geeksforgeeks.org/problems/find-pair-given-difference1559/1) — GFG practice
- [ ] SS-11 — [Find four elements with a given sum](https://www.geeksforgeeks.org/problems/find-all-four-sum-numbers1732/1) — GFG practice
- [ ] SS-12 — [Maximum sum with no two adjacent elements](https://www.geeksforgeeks.org/problems/stickler-theif-1587115621/1) — GFG practice
- [ ] SS-13 — [Count triplets with sum smaller than a given value](https://www.geeksforgeeks.org/problems/count-triplets-with-sum-smaller-than-x5549/1) — GFG practice
- [ ] SS-14 — [Merge two sorted arrays](https://www.geeksforgeeks.org/merge-two-sorted-arrays/) — GFG article
- [ ] SS-15 — [Print all zero-sum subarrays](https://www.geeksforgeeks.org/print-all-subarrays-with-0-sum/) — GFG article
- [ ] SS-16 — [Product array puzzle](https://www.geeksforgeeks.org/problems/product-array-puzzle4525/1) — GFG practice
- [ ] SS-17 — [Sort an array by set-bit count](https://www.geeksforgeeks.org/problems/sort-by-set-bit-count1153/1) — GFG practice
- [ ] SS-18 — [Minimum swaps to sort an array](https://www.geeksforgeeks.org/problems/minimum-swaps/1) — GFG practice
- [ ] SS-19 — [Bishu and Soldiers](https://www.hackerearth.com/problem/algorithm/bishu-and-soldiers/) — Original judge (not GFG/LeetCode)
- [ ] SS-20 — [Rasta and Kheshtak](https://www.geeksforgeeks.org/search/?gq=Rasta%20and%20Kheshtak) — GFG search (not a verified direct match)
- [ ] SS-21 — [Kth smallest number again](https://www.geeksforgeeks.org/search/?gq=Kth%20smallest%20number%20again) — GFG search (not a verified direct match)
- [ ] SS-22 — [Find the pivot in a sorted rotated array](https://www.geeksforgeeks.org/search-an-element-in-a-sorted-and-pivoted-array/) — GFG article
- [ ] SS-23 — [Kth element of two sorted arrays](https://www.geeksforgeeks.org/problems/k-th-element-of-two-sorted-array1317/1) — GFG practice
- [ ] SS-24 — [Aggressive cows](https://www.geeksforgeeks.org/problems/aggressive-cows/1) — GFG practice
- [ ] SS-25 — [Book allocation](https://www.geeksforgeeks.org/problems/allocate-minimum-number-of-pages0937/1) — GFG practice
- [ ] SS-26 — [EKO (SPOJ)](https://www.spoj.com/problems/EKO/) — Original judge
- [ ] SS-27 — [Job scheduling algorithm](https://www.geeksforgeeks.org/weighted-job-scheduling/) — GFG article
- [ ] SS-28 — [Missing number in an arithmetic progression](https://www.geeksforgeeks.org/problems/missing-number-in-ap2228/1) — GFG practice
- [ ] SS-29 — [Smallest number with at least n trailing zeroes in its factorial](https://www.geeksforgeeks.org/problems/smallest-factorial-number5929/1) — GFG practice
- [ ] SS-30 — [Painter’s partition](https://www.geeksforgeeks.org/problems/the-painters-partition-problem1535/1) — GFG practice
- [ ] SS-31 — [Roti Prata (SPOJ)](https://www.spoj.com/problems/PRATA/) — Original judge
- [ ] SS-32 — [Double Helix (SPOJ)](https://www.spoj.com/problems/ANARC05B/) — Original judge
- [ ] SS-33 — [Subset sums](https://www.geeksforgeeks.org/problems/subset-sums2234/1) — GFG practice
- [ ] SS-34 — [Inversion count (retained repeated entry)](https://www.geeksforgeeks.org/problems/inversion-of-array/1) — GFG practice
- [ ] SS-35 — [Implement merge sort in place](https://www.geeksforgeeks.org/in-place-merge-sort/) — GFG article
- [ ] SS-36 — [Partition and sort arrays with many repeated entries](https://www.geeksforgeeks.org/3-way-quicksort-dutch-national-flag/) — GFG article

[Back to section counts](#section-navigation-and-counts)

## Linked Lists

36 entries.

- [ ] LL-01 — [Reverse a linked list iteratively and recursively](https://www.geeksforgeeks.org/problems/reverse-a-linked-list/1) — GFG practice
- [ ] LL-02 — [Reverse a linked list in groups of a given size](https://www.geeksforgeeks.org/problems/reverse-a-linked-list-in-groups-of-given-size/1) — GFG practice
- [ ] LL-03 — [Detect a loop in a linked list](https://www.geeksforgeeks.org/problems/detect-loop-in-linked-list/1) — GFG practice
- [ ] LL-04 — [Remove a loop in a linked list](https://www.geeksforgeeks.org/problems/remove-loop-in-linked-list/1) — GFG practice
- [ ] LL-05 — [Find the starting point of a loop](https://leetcode.com/problems/linked-list-cycle-ii/) — LeetCode
- [ ] LL-06 — [Remove duplicates from a sorted linked list](https://www.geeksforgeeks.org/problems/remove-duplicate-element-from-sorted-linked-list/1) — GFG practice
- [ ] LL-07 — [Remove duplicates from an unsorted linked list](https://www.geeksforgeeks.org/problems/remove-duplicates-from-an-unsorted-linked-list/1) — GFG practice
- [ ] LL-08 — [Move the last node to the front](https://www.geeksforgeeks.org/move-last-element-to-front-of-a-given-linked-list/) — GFG article
- [ ] LL-09 — [Add one to a number represented by a linked list](https://www.geeksforgeeks.org/problems/add-1-to-a-number-represented-as-linked-list/1) — GFG practice
- [ ] LL-10 — [Add two numbers represented by linked lists](https://www.geeksforgeeks.org/problems/add-two-numbers-represented-by-linked-lists/1) — GFG practice
- [ ] LL-11 — [Intersection of two sorted linked lists](https://www.geeksforgeeks.org/problems/intersection-of-two-sorted-linked-lists/1) — GFG practice
- [ ] LL-12 — [Intersection point of two linked lists](https://www.geeksforgeeks.org/problems/intersection-point-in-y-shapped-linked-lists/1) — GFG practice
- [ ] LL-13 — [Merge sort for linked lists](https://www.geeksforgeeks.org/problems/sort-a-linked-list/1) — GFG practice
- [ ] LL-14 — [Quicksort for linked lists](https://www.geeksforgeeks.org/problems/quick-sort-on-linked-list/1) — GFG practice
- [ ] LL-15 — [Middle element of a linked list](https://www.geeksforgeeks.org/problems/finding-middle-element-in-a-linked-list/1) — GFG practice
- [ ] LL-16 — [Check whether a linked list is circular](https://www.geeksforgeeks.org/problems/circular-linked-list/1) — GFG practice
- [ ] LL-17 — [Split a circular linked list into two halves](https://www.geeksforgeeks.org/problems/split-a-circular-linked-list-into-two-halves/1) — GFG practice
- [ ] LL-18 — [Check whether a singly linked list is a palindrome](https://www.geeksforgeeks.org/problems/check-if-linked-list-is-pallindrome/1) — GFG practice
- [ ] LL-19 — [Delete from a circular linked list](https://www.geeksforgeeks.org/deletion-circular-linked-list/) — GFG article
- [ ] LL-20 — [Reverse a doubly linked list](https://www.geeksforgeeks.org/problems/reverse-a-doubly-linked-list/1) — GFG practice
- [ ] LL-21 — [Pairs with a given sum in a doubly linked list](https://www.geeksforgeeks.org/find-pairs-given-sum-doubly-linked-list/) — GFG article
- [ ] LL-22 — [Count triplets with a given sum in a sorted doubly linked list](https://www.geeksforgeeks.org/count-triplets-sorted-doubly-linked-list-whose-sum-equal-given-value-x/) — GFG article
- [ ] LL-23 — [Sort a k-sorted doubly linked list](https://www.geeksforgeeks.org/sort-k-sorted-doubly-linked-list/) — GFG article
- [ ] LL-24 — [Rotate a doubly linked list by N nodes](https://www.geeksforgeeks.org/rotate-doubly-linked-list-n-nodes/) — GFG article
- [ ] LL-25 — [Rotate a doubly linked list in groups of a given size](https://www.geeksforgeeks.org/search/?gq=rotate%20doubly%20linked%20list%20in%20groups) — GFG search (ambiguous sheet wording)
- [ ] LL-26 — [Can a linked list be reversed in less than O(n)? (conceptual)](https://www.geeksforgeeks.org/search/?gq=Can%20a%20linked%20list%20be%20reversed%20in%20less%20than%20O%28n%29%3F%20%28conceptual%29) — GFG search (not a verified direct match)
- [ ] LL-27 — [Why quicksort for arrays and merge sort for linked lists? (conceptual)](https://www.geeksforgeeks.org/why-quick-sort-preferred-for-arrays-and-merge-sort-for-linked-lists/) — GFG article
- [ ] LL-28 — [Flatten a linked list](https://www.geeksforgeeks.org/problems/flattening-a-linked-list/1) — GFG practice
- [ ] LL-29 — [Sort a linked list of 0s, 1s and 2s](https://www.geeksforgeeks.org/problems/given-a-linked-list-of-0s-1s-and-2s-sort-it/1) — GFG practice
- [ ] LL-30 — [Clone a linked list with next and random pointers](https://leetcode.com/problems/copy-list-with-random-pointer/) — LeetCode
- [ ] LL-31 — [Merge K sorted linked lists](https://leetcode.com/problems/merge-k-sorted-lists/) — LeetCode
- [ ] LL-32 — [Multiply two numbers represented by linked lists](https://www.geeksforgeeks.org/problems/multiply-two-linked-lists/1) — GFG practice
- [ ] LL-33 — [Delete nodes with a greater value on the right](https://www.geeksforgeeks.org/problems/delete-nodes-having-greater-value-on-right/1) — GFG practice
- [ ] LL-34 — [Segregate even and odd nodes](https://www.geeksforgeeks.org/problems/segregate-even-and-odd-nodes-in-a-linked-list/1) — GFG practice
- [ ] LL-35 — [Nth node from the end](https://www.geeksforgeeks.org/problems/nth-node-from-end-of-linked-list/1) — GFG practice
- [ ] LL-36 — [First non-repeating character in a stream](https://www.geeksforgeeks.org/problems/first-non-repeating-character-in-a-stream/1) — GFG practice

[Back to section counts](#section-navigation-and-counts)

## Binary Trees

35 entries.

- [ ] BT-01 — [Level-order traversal](https://www.geeksforgeeks.org/problems/level-order-traversal/1) — GFG practice
- [ ] BT-02 — [Reverse level-order traversal](https://www.geeksforgeeks.org/problems/reverse-level-order-traversal/1) — GFG practice
- [ ] BT-03 — [Height of a tree](https://www.geeksforgeeks.org/problems/height-of-binary-tree/1) — GFG practice
- [ ] BT-04 — [Diameter of a tree](https://www.geeksforgeeks.org/problems/diameter-of-binary-tree/1) — GFG practice
- [ ] BT-05 — [Mirror a tree](https://www.geeksforgeeks.org/problems/mirror-tree/1) — GFG practice
- [ ] BT-06 — [Inorder traversal: recursive and iterative](https://www.geeksforgeeks.org/problems/inorder-traversal/1) — GFG practice
- [ ] BT-07 — [Preorder traversal: recursive and iterative](https://www.geeksforgeeks.org/problems/preorder-traversal/1) — GFG practice
- [ ] BT-08 — [Postorder traversal: recursive and iterative](https://www.geeksforgeeks.org/problems/postorder-traversal/1) — GFG practice
- [ ] BT-09 — [Left view of a tree](https://www.geeksforgeeks.org/problems/left-view-of-binary-tree/1) — GFG practice
- [ ] BT-10 — [Right view of a tree](https://www.geeksforgeeks.org/problems/right-view-of-binary-tree/1) — GFG practice
- [ ] BT-11 — [Top view of a tree](https://www.geeksforgeeks.org/problems/top-view-of-binary-tree/1) — GFG practice
- [ ] BT-12 — [Bottom view of a tree](https://www.geeksforgeeks.org/problems/bottom-view-of-binary-tree/1) — GFG practice
- [ ] BT-13 — [Zigzag traversal](https://www.geeksforgeeks.org/problems/zigzag-tree-traversal/1) — GFG practice
- [ ] BT-14 — [Check whether a tree is balanced](https://www.geeksforgeeks.org/problems/check-for-balanced-tree/1) — GFG practice
- [ ] BT-15 — [Diagonal traversal](https://www.geeksforgeeks.org/problems/diagonal-traversal-of-binary-tree/1) — GFG practice
- [ ] BT-16 — [Boundary traversal](https://www.geeksforgeeks.org/problems/boundary-traversal-of-binary-tree/1) — GFG practice
- [ ] BT-17 — [Construct a binary tree from a bracketed string](https://www.geeksforgeeks.org/construct-binary-tree-string-bracket-representation/) — GFG article
- [ ] BT-18 — [Convert a binary tree to a doubly linked list](https://www.geeksforgeeks.org/problems/binary-tree-to-dll/1) — GFG practice
- [ ] BT-19 — [Convert a binary tree to a sum tree](https://www.geeksforgeeks.org/problems/transform-to-sum-tree/1) — GFG practice
- [ ] BT-20 — [Construct a tree from inorder and preorder traversals](https://www.geeksforgeeks.org/problems/construct-tree-1/1) — GFG practice
- [ ] BT-21 — [Minimum swaps to convert a binary tree to a BST](https://www.geeksforgeeks.org/minimum-swap-required-convert-binary-tree-binary-search-tree/) — GFG article
- [ ] BT-22 — [Check whether a tree is a sum tree](https://www.geeksforgeeks.org/problems/sum-tree/1) — GFG practice
- [ ] BT-23 — [Check whether all leaves are at the same level](https://www.geeksforgeeks.org/problems/leaf-at-same-level/1) — GFG practice
- [ ] BT-24 — [Detect duplicate subtrees of size two or more](https://www.geeksforgeeks.org/problems/duplicate-subtree-in-binary-tree/1) — GFG practice
- [ ] BT-25 — [Check whether two trees are mirrors](https://www.geeksforgeeks.org/check-if-two-trees-are-mirror/) — GFG article
- [ ] BT-26 — [Sum of nodes on the longest root-to-leaf path](https://www.geeksforgeeks.org/problems/sum-of-the-longest-bloodline-of-a-tree/1) — GFG practice
- [ ] BT-27 — [Check whether a graph is a tree](https://www.geeksforgeeks.org/check-given-graph-tree/) — GFG article
- [ ] BT-28 — [Largest subtree sum](https://www.geeksforgeeks.org/find-largest-subtree-sum-tree/) — GFG article
- [ ] BT-29 — [Maximum node sum with no two adjacent nodes](https://www.geeksforgeeks.org/problems/maximum-sum-of-non-adjacent-nodes/1) — GFG practice
- [ ] BT-30 — [Print all K-sum paths](https://www.geeksforgeeks.org/print-k-sum-paths-binary-tree/) — GFG article
- [ ] BT-31 — [Lowest common ancestor in a binary tree](https://www.geeksforgeeks.org/problems/lowest-common-ancestor-in-a-binary-tree/1) — GFG practice
- [ ] BT-32 — [Distance between two nodes](https://www.geeksforgeeks.org/problems/min-distance-between-two-given-nodes-of-a-binary-tree/1) — GFG practice
- [ ] BT-33 — [Kth ancestor of a node](https://www.geeksforgeeks.org/problems/kth-ancestor-in-a-tree/1) — GFG practice
- [ ] BT-34 — [Find all duplicate subtrees](https://leetcode.com/problems/find-duplicate-subtrees/) — LeetCode
- [ ] BT-35 — [Tree isomorphism](https://www.geeksforgeeks.org/problems/check-if-tree-is-isomorphic/1) — GFG practice

[Back to section counts](#section-navigation-and-counts)

## Binary Search Trees

22 entries.

- [ ] BST-01 — [Search for a value in a BST](https://leetcode.com/problems/search-in-a-binary-search-tree/) — LeetCode
- [ ] BST-02 — [Delete a node from a BST](https://leetcode.com/problems/delete-node-in-a-bst/) — LeetCode
- [ ] BST-03 — [Find minimum and maximum in a BST](https://www.geeksforgeeks.org/find-the-minimum-element-in-a-binary-search-tree/) — GFG article
- [ ] BST-04 — [Inorder predecessor and successor](https://www.geeksforgeeks.org/problems/predecessor-and-successor/1) — GFG practice
- [ ] BST-05 — [Check whether a tree is a BST](https://www.geeksforgeeks.org/problems/check-for-bst/1) — GFG practice
- [ ] BST-06 — [Populate inorder successors of all nodes](https://www.geeksforgeeks.org/problems/populate-inorder-successor-for-all-nodes/1) — GFG practice
- [ ] BST-07 — [Lowest common ancestor in a BST](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-search-tree/) — LeetCode
- [ ] BST-08 — [Construct a BST from preorder traversal](https://leetcode.com/problems/construct-binary-search-tree-from-preorder-traversal/) — LeetCode
- [ ] BST-09 — [Convert a binary tree to a BST](https://www.geeksforgeeks.org/problems/binary-tree-to-bst/1) — GFG practice
- [ ] BST-10 — [Balance a BST](https://leetcode.com/problems/balance-a-binary-search-tree/) — LeetCode
- [ ] BST-11 — [Merge two BSTs](https://www.geeksforgeeks.org/merge-two-balanced-binary-search-trees/) — GFG article
- [ ] BST-12 — [Kth largest element in a BST](https://www.geeksforgeeks.org/problems/kth-largest-element-in-bst/1) — GFG practice
- [ ] BST-13 — [Kth smallest element in a BST](https://leetcode.com/problems/kth-smallest-element-in-a-bst/) — LeetCode
- [ ] BST-14 — [Count pairs from two BSTs with a given sum](https://www.geeksforgeeks.org/problems/brothers-from-different-root/1) — GFG practice
- [ ] BST-15 — [Median of a BST in O(n) time and O(1) space](https://www.geeksforgeeks.org/find-median-bst-time-o1-space/) — GFG article
- [ ] BST-16 — [Count BST nodes in a given range](https://www.geeksforgeeks.org/problems/count-bst-nodes-that-lie-in-a-given-range/1) — GFG practice
- [ ] BST-17 — [Replace each element by the least greater element on its right](https://www.geeksforgeeks.org/replace-every-element-with-the-least-greater-element-on-its-right/) — GFG article
- [ ] BST-18 — [Find conflicting appointments](https://www.geeksforgeeks.org/given-n-appointments-find-conflicting-appointments/) — GFG article
- [ ] BST-19 — [Check whether a preorder sequence represents a BST](https://www.geeksforgeeks.org/check-if-a-given-array-can-represent-preorder-traversal-of-binary-search-tree/) — GFG article
- [ ] BST-20 — [Check whether a BST contains a dead end](https://www.geeksforgeeks.org/problems/check-whether-bst-contains-dead-end/1) — GFG practice
- [ ] BST-21 — [Largest BST in a binary tree](https://www.geeksforgeeks.org/problems/largest-bst/1) — GFG practice
- [ ] BST-22 — [Flatten a BST to a sorted list](https://www.geeksforgeeks.org/flatten-bst-to-sorted-list-increasing-order/) — GFG article

[Back to section counts](#section-navigation-and-counts)

## Greedy

35 entries.

- [ ] GR-01 — [Activity selection](https://www.geeksforgeeks.org/problems/activity-selection-1587115620/1) — GFG practice
- [ ] GR-02 — [Job sequencing](https://www.geeksforgeeks.org/problems/job-sequencing-problem-1587115620/1) — GFG practice
- [ ] GR-03 — [Huffman coding](https://www.geeksforgeeks.org/problems/huffman-encoding3345/1) — GFG practice
- [ ] GR-04 — [Water connection problem](https://www.geeksforgeeks.org/problems/water-connection-problem5822/1) — GFG practice
- [ ] GR-05 — [Fractional knapsack](https://www.geeksforgeeks.org/problems/fractional-knapsack-1587115620/1) — GFG practice
- [ ] GR-06 — [Minimum number of coins using a greedy algorithm](https://www.geeksforgeeks.org/greedy-algorithm-to-find-minimum-number-of-coins/) — GFG article
- [ ] GR-07 — [Maximum trains that can be provided stoppages](https://www.geeksforgeeks.org/maximum-trains-stoppage-can-provided/) — GFG article
- [ ] GR-08 — [Minimum railway platforms](https://www.geeksforgeeks.org/problems/minimum-platforms-1587115620/1) — GFG practice
- [ ] GR-09 — [Buy maximum stocks when i stocks can be bought on day i](https://www.geeksforgeeks.org/buy-maximum-stocks-stocks-can-bought-th-day/) — GFG article
- [ ] GR-10 — [Minimum and maximum cost to buy all candies](https://www.geeksforgeeks.org/problems/shop-in-candy-store1145/1) — GFG practice
- [ ] GR-11 — [Minimise cash flow among friends](https://www.geeksforgeeks.org/minimize-cash-flow-among-given-set-friends-borrowed-money/) — GFG article
- [ ] GR-12 — [Minimum cost to cut a board into squares](https://www.geeksforgeeks.org/minimum-cost-cut-board-squares/) — GFG article
- [ ] GR-13 — [Check whether survival on an island is possible](https://www.geeksforgeeks.org/problems/check-if-it-is-possible-to-survive-on-island4922/1) — GFG practice
- [ ] GR-14 — [Maximum meetings in one room](https://www.geeksforgeeks.org/problems/n-meetings-in-one-room-1587115620/1) — GFG practice
- [ ] GR-15 — [Maximum-product subset](https://www.geeksforgeeks.org/maximum-product-subset-array/) — GFG article
- [ ] GR-16 — [Maximise array sum after K negations](https://www.geeksforgeeks.org/problems/maximize-sum-after-k-negations1149/1) — GFG practice
- [ ] GR-17 — [Maximise sum of arr[i] * i](https://www.geeksforgeeks.org/problems/maximize-arrii-of-an-array0026/1) — GFG practice
- [ ] GR-18 — [Maximum sum of absolute differences](https://www.geeksforgeeks.org/maximum-sum-absolute-difference-array/) — GFG article
- [ ] GR-19 — [Maximum sum of consecutive differences in a circular array](https://www.geeksforgeeks.org/maximum-sum-consecutive-differences-circular-array/) — GFG article
- [ ] GR-20 — [Minimum sum of absolute differences between paired arrays](https://www.geeksforgeeks.org/minimum-sum-absolute-difference-pairs-two-arrays/) — GFG article
- [ ] GR-21 — [Shortest Job First CPU scheduling](https://www.geeksforgeeks.org/program-for-shortest-job-first-or-sjf-cpu-scheduling-set-1-non-preemptive/) — GFG article
- [ ] GR-22 — [Least Recently Used page replacement](https://www.geeksforgeeks.org/program-for-least-recently-used-lru-page-replacement-algorithm/) — GFG article
- [ ] GR-23 — [Smallest subset with sum greater than remaining elements](https://www.geeksforgeeks.org/problems/smallest-subset-with-greater-sum/1) — GFG practice
- [ ] GR-24 — [Chocolate distribution (retained repeated entry)](https://www.geeksforgeeks.org/problems/chocolate-distribution-problem/1) — GFG practice
- [ ] GR-25 — [Defense of a Kingdom (SPOJ)](https://www.spoj.com/problems/DEFKIN/) — Original judge
- [ ] GR-26 — [Die Hard (SPOJ)](https://www.spoj.com/problems/DIEHARD/) — Original judge
- [ ] GR-27 — [Wine trading in Gergovia (SPOJ)](https://www.spoj.com/problems/GERGOVIA/) — Original judge
- [ ] GR-28 — [Picking Up Chicks](https://www.geeksforgeeks.org/search/?gq=Picking%20Up%20Chicks) — GFG search (not a verified direct match)
- [ ] GR-29 — [Chocolate cutting (SPOJ)](https://www.spoj.com/problems/CHOCOLA/) — Original judge
- [ ] GR-30 — [Arranging Amplifiers (SPOJ)](https://www.spoj.com/problems/ARRANGE/) — Original judge
- [ ] GR-31 — [K-centres problem](https://www.geeksforgeeks.org/greedy-approximate-algorithm-for-k-centers-problem/) — GFG article
- [ ] GR-32 — [Minimum cost of ropes](https://www.geeksforgeeks.org/problems/minimum-cost-of-ropes-1587115620/1) — GFG practice
- [ ] GR-33 — [Smallest number with a given digit count and digit sum](https://www.geeksforgeeks.org/problems/smallest-number5829/1) — GFG practice
- [ ] GR-34 — [Rearrange a string so adjacent characters differ](https://leetcode.com/problems/reorganize-string/) — LeetCode
- [ ] GR-35 — [Maximum possible equal sum of three stacks](https://www.geeksforgeeks.org/find-maximum-sum-possible-equal-sum-three-stacks/) — GFG article

[Back to section counts](#section-navigation-and-counts)

## Backtracking

19 entries.

- [ ] BK-01 — [Rat in a maze](https://www.geeksforgeeks.org/problems/rat-in-a-maze-problem/1) — GFG practice
- [ ] BK-02 — [Print all solutions to N-Queens](https://leetcode.com/problems/n-queens/) — LeetCode
- [ ] BK-03 — [Word break using backtracking](https://www.geeksforgeeks.org/problems/word-break-part-2/1) — GFG practice
- [ ] BK-04 — [Remove invalid parentheses](https://leetcode.com/problems/remove-invalid-parentheses/) — LeetCode
- [ ] BK-05 — [Sudoku solver](https://leetcode.com/problems/sudoku-solver/) — LeetCode
- [ ] BK-06 — [M-colouring problem](https://www.geeksforgeeks.org/problems/m-coloring-problem-1587115620/1) — GFG practice
- [ ] BK-07 — [All palindromic partitions of a string](https://leetcode.com/problems/palindrome-partitioning/) — LeetCode
- [ ] BK-08 — [Subset sum](https://www.geeksforgeeks.org/problems/subset-sum-problem-1611555638/1) — GFG practice
- [ ] BK-09 — [Knight’s tour](https://www.geeksforgeeks.org/the-knights-tour-problem/) — GFG article
- [ ] BK-10 — [Tug of war](https://www.geeksforgeeks.org/tug-of-war/) — GFG article
- [ ] BK-11 — [Shortest safe route through landmines](https://www.geeksforgeeks.org/find-shortest-safe-route-in-a-path-with-landmines/) — GFG article
- [ ] BK-12 — [Combination sum](https://www.geeksforgeeks.org/problems/combination-sum-1587115620/1) — GFG practice
- [ ] BK-13 — [Maximum number with at most K swaps](https://www.geeksforgeeks.org/problems/largest-number-in-k-swaps-1587115620/1) — GFG practice
- [ ] BK-14 — [Print all string permutations](https://www.geeksforgeeks.org/problems/permutations-of-a-given-string2041/1) — GFG practice
- [ ] BK-15 — [Path longer than k from a source](https://www.geeksforgeeks.org/find-if-there-is-a-path-of-more-than-k-length-from-a-source/) — GFG article
- [ ] BK-16 — [Longest route in a matrix with hurdles](https://www.geeksforgeeks.org/longest-possible-route-in-a-matrix-with-hurdles/) — GFG article
- [ ] BK-17 — [All paths from top-left to bottom-right in an m x n matrix](https://www.geeksforgeeks.org/print-all-possible-paths-from-top-left-to-bottom-right-of-a-mxn-matrix/) — GFG article
- [ ] BK-18 — [Partition into K subsets of equal sum](https://leetcode.com/problems/partition-to-k-equal-sum-subsets/) — LeetCode
- [ ] BK-19 — [Kth permutation sequence of the first N natural numbers](https://leetcode.com/problems/permutation-sequence/) — LeetCode

[Back to section counts](#section-navigation-and-counts)

## Stacks and Queues

38 entries.

- [ ] SQ-01 — [Implement a stack from scratch](https://www.geeksforgeeks.org/problems/implement-stack-using-array/1) — GFG practice
- [ ] SQ-02 — [Implement a queue from scratch](https://www.geeksforgeeks.org/problems/implement-queue-using-array/1) — GFG practice
- [ ] SQ-03 — [Implement two stacks in one array](https://www.geeksforgeeks.org/problems/implement-two-stacks-in-an-array/1) — GFG practice
- [ ] SQ-04 — [Find the middle element of a stack](https://www.geeksforgeeks.org/design-a-stack-with-find-middle-operation/) — GFG article
- [ ] SQ-05 — [Implement N stacks in one array](https://www.geeksforgeeks.org/efficiently-implement-k-stacks-single-array/) — GFG article
- [ ] SQ-06 — [Check balanced parentheses](https://www.geeksforgeeks.org/problems/parenthesis-checker2744/1) — GFG practice
- [ ] SQ-07 — [Reverse a string using a stack](https://www.geeksforgeeks.org/problems/reverse-a-string-using-stack/1) — GFG practice
- [ ] SQ-08 — [Stack with getMin() in O(1) time and O(1) extra space](https://www.geeksforgeeks.org/design-a-stack-that-supports-getmin-in-o1-time-and-o1-extra-space/) — GFG article
- [ ] SQ-09 — [Next greater element](https://www.geeksforgeeks.org/problems/next-larger-element/1) — GFG practice
- [ ] SQ-10 — [Celebrity problem](https://www.geeksforgeeks.org/problems/the-celebrity-problem/1) — GFG practice
- [ ] SQ-11 — [Evaluate an arithmetic expression](https://www.geeksforgeeks.org/expression-evaluation/) — GFG article
- [ ] SQ-12 — [Evaluate a postfix expression](https://www.geeksforgeeks.org/problems/evaluation-of-postfix-expression/1) — GFG practice
- [ ] SQ-13 — [Insert an element at the bottom of a stack without another data structure](https://www.geeksforgeeks.org/program-to-insert-an-element-at-the-bottom-of-a-stack/) — GFG article
- [ ] SQ-14 — [Reverse a stack using recursion](https://www.geeksforgeeks.org/reverse-a-stack-using-recursion/) — GFG article
- [ ] SQ-15 — [Sort a stack using recursion](https://www.geeksforgeeks.org/problems/sort-a-stack/1) — GFG practice
- [ ] SQ-16 — [Merge overlapping intervals](https://leetcode.com/problems/merge-intervals/) — LeetCode
- [ ] SQ-17 — [Largest rectangle in a histogram](https://leetcode.com/problems/largest-rectangle-in-histogram/) — LeetCode
- [ ] SQ-18 — [Longest valid parentheses substring](https://leetcode.com/problems/longest-valid-parentheses/) — LeetCode
- [ ] SQ-19 — [Detect redundant brackets](https://www.geeksforgeeks.org/problems/expression-contains-redundant-bracket-or-not/1) — GFG practice
- [ ] SQ-20 — [Implement a stack using queues](https://leetcode.com/problems/implement-stack-using-queues/) — LeetCode
- [ ] SQ-21 — [Implement a stack using a deque](https://www.geeksforgeeks.org/implement-stack-queue-using-deque/) — GFG article
- [ ] SQ-22 — [Check whether an array is a stack permutation](https://www.geeksforgeeks.org/problems/stack-permutations/1) — GFG practice
- [ ] SQ-23 — [Implement a queue using stacks](https://leetcode.com/problems/implement-queue-using-stacks/) — LeetCode
- [ ] SQ-24 — [Implement N queues in one array](https://www.geeksforgeeks.org/efficiently-implement-k-queues-single-array/) — GFG article
- [ ] SQ-25 — [Implement a circular queue](https://leetcode.com/problems/design-circular-queue/) — LeetCode
- [ ] SQ-26 — [LRU cache](https://leetcode.com/problems/lru-cache/) — LeetCode
- [ ] SQ-27 — [Reverse a queue using recursion](https://www.geeksforgeeks.org/problems/queue-reversal/1) — GFG practice
- [ ] SQ-28 — [Reverse the first K elements of a queue](https://www.geeksforgeeks.org/problems/reverse-first-k-elements-of-queue/1) — GFG practice
- [ ] SQ-29 — [Interleave the first and second halves of a queue](https://www.geeksforgeeks.org/interleave-first-half-queue-second-half/) — GFG article
- [ ] SQ-30 — [First circular tour visiting all petrol pumps](https://www.geeksforgeeks.org/find-a-tour-that-visits-all-stations/) — GFG article
- [ ] SQ-31 — [Minimum time to rot all oranges](https://leetcode.com/problems/rotting-oranges/) — LeetCode
- [ ] SQ-32 — [Distance to nearest cell containing 1](https://www.geeksforgeeks.org/problems/distance-of-nearest-cell-having-1/1) — GFG practice
- [ ] SQ-33 — [First negative integer in every window of size K](https://www.geeksforgeeks.org/problems/first-negative-integer-in-every-window-of-size-k/1) — GFG practice
- [ ] SQ-34 — [Check whether levels of two trees are anagrams](https://www.geeksforgeeks.org/check-if-all-levels-of-two-trees-are-anagrams-or-not/) — GFG article
- [ ] SQ-35 — [Sum of minimum and maximum in all windows of size K](https://www.geeksforgeeks.org/sum-minimum-maximum-elements-subarrays-size-k/) — GFG article
- [ ] SQ-36 — [Minimum sum of squared character frequencies after K removals](https://www.geeksforgeeks.org/problems/game-with-string4100/1) — GFG practice
- [ ] SQ-37 — [First non-repeating character in a stream using a queue](https://www.geeksforgeeks.org/problems/first-non-repeating-character-in-a-stream/1) — GFG practice
- [ ] SQ-38 — [Next smaller element](https://www.geeksforgeeks.org/problems/immediate-smaller-element1142/1) — GFG practice

[Back to section counts](#section-navigation-and-counts)

## Heap

18 entries.

- [ ] HP-01 — [Implement max-heap and min-heap using arrays and recursion](https://www.geeksforgeeks.org/binary-heap/) — GFG article
- [ ] HP-02 — [Heap sort](https://www.geeksforgeeks.org/problems/heap-sort/1) — GFG practice
- [ ] HP-03 — [Maximum of all subarrays of size K](https://leetcode.com/problems/sliding-window-maximum/) — LeetCode
- [ ] HP-04 — [K largest elements in an array](https://www.geeksforgeeks.org/problems/k-largest-elements4206/1) — GFG practice
- [ ] HP-05 — [Kth smallest and largest element in an unsorted array](https://www.geeksforgeeks.org/kth-smallest-largest-element-in-unsorted-array/) — GFG article
- [ ] HP-06 — [Merge K sorted arrays](https://www.geeksforgeeks.org/problems/merge-k-sorted-arrays/1) — GFG practice
- [ ] HP-07 — [Merge two binary max-heaps](https://www.geeksforgeeks.org/problems/merge-two-binary-max-heap0144/1) — GFG practice
- [ ] HP-08 — [Kth largest contiguous subarray sum](https://www.geeksforgeeks.org/k-th-largest-sum-contiguous-subarray/) — GFG article
- [ ] HP-09 — [Reorganise a string (LeetCode)](https://leetcode.com/problems/reorganize-string/) — LeetCode
- [ ] HP-10 — [Merge K sorted linked lists](https://leetcode.com/problems/merge-k-sorted-lists/) — LeetCode
- [ ] HP-11 — [Smallest range covering elements of K lists](https://leetcode.com/problems/smallest-range-covering-elements-from-k-lists/) — LeetCode
- [ ] HP-12 — [Median in a stream](https://leetcode.com/problems/find-median-from-data-stream/) — LeetCode
- [ ] HP-13 — [Check whether a binary tree is a heap](https://www.geeksforgeeks.org/problems/is-binary-tree-heap/1) — GFG practice
- [ ] HP-14 — [Connect N ropes with minimum cost](https://www.geeksforgeeks.org/problems/minimum-cost-of-ropes-1587115620/1) — GFG practice
- [ ] HP-15 — [Convert a BST to a min-heap](https://www.geeksforgeeks.org/convert-bst-min-heap/) — GFG article
- [ ] HP-16 — [Convert a min-heap to a max-heap](https://www.geeksforgeeks.org/convert-min-heap-to-max-heap/) — GFG article
- [ ] HP-17 — [Rearrange characters so adjacent characters differ (retained repeat)](https://leetcode.com/problems/reorganize-string/) — LeetCode
- [ ] HP-18 — [Minimum sum of two numbers formed from array digits](https://www.geeksforgeeks.org/problems/minimum-sum4058/1) — GFG practice

[Back to section counts](#section-navigation-and-counts)

## Graphs

44 entries.

- [ ] GP-01 — [Create and print a graph](https://www.geeksforgeeks.org/graph-and-its-representations/) — GFG article
- [ ] GP-02 — [Breadth-first search](https://www.geeksforgeeks.org/problems/bfs-traversal-of-graph/1) — GFG practice
- [ ] GP-03 — [Depth-first search](https://www.geeksforgeeks.org/problems/depth-first-traversal-for-a-graph/1) — GFG practice
- [ ] GP-04 — [Detect a cycle in a directed graph using BFS or DFS](https://www.geeksforgeeks.org/problems/detect-cycle-in-a-directed-graph/1) — GFG practice
- [ ] GP-05 — [Detect a cycle in an undirected graph using BFS or DFS](https://www.geeksforgeeks.org/problems/detect-cycle-in-an-undirected-graph/1) — GFG practice
- [ ] GP-06 — [Search in a maze](https://www.geeksforgeeks.org/problems/rat-in-a-maze-problem/1) — GFG practice
- [ ] GP-07 — [Minimum moves by a knight](https://www.geeksforgeeks.org/problems/steps-by-knight5927/1) — GFG practice
- [ ] GP-08 — [Flood fill](https://leetcode.com/problems/flood-fill/) — LeetCode
- [ ] GP-09 — [Clone a graph](https://leetcode.com/problems/clone-graph/) — LeetCode
- [ ] GP-10 — [Make a network connected](https://leetcode.com/problems/number-of-operations-to-make-network-connected/) — LeetCode
- [ ] GP-11 — [Word ladder](https://leetcode.com/problems/word-ladder/) — LeetCode
- [ ] GP-12 — [Dijkstra’s algorithm](https://www.geeksforgeeks.org/problems/implementing-dijkstra-set-1-adjacency-matrix/1) — GFG practice
- [ ] GP-13 — [Topological sort](https://www.geeksforgeeks.org/problems/topological-sort/1) — GFG practice
- [ ] GP-14 — [Minimum completion time for jobs in a DAG](https://www.geeksforgeeks.org/minimum-time-taken-by-each-job-to-be-completed-given-by-a-directed-acyclic-graph/) — GFG article
- [ ] GP-15 — [Check whether all tasks can be completed given dependencies](https://leetcode.com/problems/course-schedule/) — LeetCode
- [ ] GP-16 — [Number of islands](https://leetcode.com/problems/number-of-islands/) — LeetCode
- [ ] GP-17 — [Alien dictionary character order](https://www.geeksforgeeks.org/problems/alien-dictionary/1) — GFG practice
- [ ] GP-18 — [Kruskal’s minimum spanning tree algorithm](https://www.geeksforgeeks.org/kruskals-minimum-spanning-tree-algorithm-greedy-algo-2/) — GFG article
- [ ] GP-19 — [Prim’s minimum spanning tree algorithm](https://www.geeksforgeeks.org/prims-minimum-spanning-tree-mst-greedy-algo-5/) — GFG article
- [ ] GP-20 — [Total number of spanning trees](https://www.geeksforgeeks.org/total-number-spanning-trees-graph/) — GFG article
- [ ] GP-21 — [Bellman–Ford algorithm](https://www.geeksforgeeks.org/problems/distance-from-the-source-bellman-ford-algorithm/1) — GFG practice
- [ ] GP-22 — [Floyd–Warshall algorithm](https://www.geeksforgeeks.org/problems/implementing-floyd-warshall2042/1) — GFG practice
- [ ] GP-23 — [Travelling salesman problem](https://www.geeksforgeeks.org/travelling-salesman-problem-using-dynamic-programming/) — GFG article
- [ ] GP-24 — [Graph colouring](https://www.geeksforgeeks.org/graph-coloring-applications/) — GFG article
- [ ] GP-25 — [Snakes and ladders](https://leetcode.com/problems/snakes-and-ladders/) — LeetCode
- [ ] GP-26 — [Find bridges in a graph](https://www.geeksforgeeks.org/bridge-in-a-graph/) — GFG article
- [ ] GP-27 — [Strongly connected components using Kosaraju’s algorithm](https://www.geeksforgeeks.org/problems/strongly-connected-components-kosarajus-algo/1) — GFG practice
- [ ] GP-28 — [Check whether a graph is bipartite](https://leetcode.com/problems/is-graph-bipartite/) — LeetCode
- [ ] GP-29 — [Detect a negative-weight cycle](https://www.geeksforgeeks.org/problems/negative-weight-cycle3504/1) — GFG practice
- [ ] GP-30 — [Longest path in a DAG](https://www.geeksforgeeks.org/find-longest-path-directed-acyclic-graph/) — GFG article
- [ ] GP-31 — [Journey to the Moon](https://www.hackerrank.com/challenges/journey-to-the-moon/problem) — Original judge (not GFG/LeetCode)
- [ ] GP-32 — [Cheapest flights within K stops](https://leetcode.com/problems/cheapest-flights-within-k-stops/) — LeetCode
- [ ] GP-33 — [Oliver and the Game](https://www.geeksforgeeks.org/search/?gq=Oliver%20and%20the%20Game) — GFG search (not a verified direct match)
- [ ] GP-34 — [Water jug using BFS](https://www.geeksforgeeks.org/water-jug-problem-using-bfs/) — GFG article
- [ ] GP-35 — [Water jug using BFS (retained duplicate entry)](https://www.geeksforgeeks.org/water-jug-problem-using-bfs/) — GFG article
- [ ] GP-36 — [Path longer than K from a source](https://www.geeksforgeeks.org/find-if-there-is-a-path-of-more-than-k-length-from-a-source/) — GFG article
- [ ] GP-37 — [M-colouring problem](https://www.geeksforgeeks.org/problems/m-coloring-problem-1587115620/1) — GFG practice
- [ ] GP-38 — [Minimum edge reversals from source to destination](https://www.geeksforgeeks.org/minimum-edges-reverse-make-path-source-destination/) — GFG article
- [ ] GP-39 — [Traverse each edge once: Seven Bridges / Euler paths](https://www.geeksforgeeks.org/eulerian-path-and-circuit/) — GFG article
- [ ] GP-40 — [Vertex cover](https://www.geeksforgeeks.org/vertex-cover-problem-set-1-introduction-approximate-algorithm-2/) — GFG article
- [ ] GP-41 — [Chinese postman / route inspection](https://www.geeksforgeeks.org/chinese-postman-route-inspection-set-1-introduction/) — GFG article
- [ ] GP-42 — [Count triangles in directed and undirected graphs](https://www.geeksforgeeks.org/number-of-triangles-in-directed-and-undirected-graphs/) — GFG article
- [ ] GP-43 — [Minimise cash flow among friends](https://www.geeksforgeeks.org/minimize-cash-flow-among-given-set-friends-borrowed-money/) — GFG article
- [ ] GP-44 — [Two-clique problem](https://www.geeksforgeeks.org/two-clique-problem-check-graph-can-divided-two-cliques/) — GFG article

[Back to section counts](#section-navigation-and-counts)

## Trie

6 entries.

- [ ] TR-01 — [Construct a trie from scratch](https://leetcode.com/problems/implement-trie-prefix-tree/) — LeetCode
- [ ] TR-02 — [Shortest unique prefix for every word](https://www.geeksforgeeks.org/problems/shortest-unique-prefix-for-every-word/1) — GFG practice
- [ ] TR-03 — [Word break using a trie](https://www.geeksforgeeks.org/word-break-problem-trie-solution/) — GFG article
- [ ] TR-04 — [Group anagrams using a trie](https://www.geeksforgeeks.org/given-a-sequence-of-words-print-all-anagrams-together/) — GFG article
- [ ] TR-05 — [Implement a phone directory](https://www.geeksforgeeks.org/problems/phone-directory4628/1) — GFG practice
- [ ] TR-06 — [Print unique rows in a boolean matrix](https://www.geeksforgeeks.org/problems/unique-rows-in-boolean-matrix/1) — GFG practice

[Back to section counts](#section-navigation-and-counts)

## Dynamic Programming

60 entries.

- [ ] DP-01 — [Coin change: number of ways](https://www.geeksforgeeks.org/problems/coin-change2448/1) — GFG practice
- [ ] DP-02 — [0/1 knapsack](https://www.geeksforgeeks.org/problems/0-1-knapsack-problem0945/1) — GFG practice
- [ ] DP-03 — [Binomial coefficient](https://www.geeksforgeeks.org/problems/ncr1019/1) — GFG practice
- [ ] DP-04 — [Permutation coefficient](https://www.geeksforgeeks.org/permutation-coefficient/) — GFG article
- [ ] DP-05 — [Nth Catalan number](https://www.geeksforgeeks.org/problems/nth-catalan-number0817/1) — GFG practice
- [ ] DP-06 — [Matrix chain multiplication](https://www.geeksforgeeks.org/problems/matrix-chain-multiplication0303/1) — GFG practice
- [ ] DP-07 — [Edit distance](https://www.geeksforgeeks.org/problems/edit-distance3702/1) — GFG practice
- [ ] DP-08 — [Subset sum](https://www.geeksforgeeks.org/problems/subset-sum-problem-1611555638/1) — GFG practice
- [ ] DP-09 — [Friends pairing](https://www.geeksforgeeks.org/problems/friends-pairing-problem5425/1) — GFG practice
- [ ] DP-10 — [Gold mine](https://www.geeksforgeeks.org/problems/gold-mine-problem2608/1) — GFG practice
- [ ] DP-11 — [Assembly line scheduling](https://www.geeksforgeeks.org/assembly-line-scheduling-dp-34/) — GFG article
- [ ] DP-12 — [Painting the fence](https://www.geeksforgeeks.org/problems/painting-the-fence3727/1) — GFG practice
- [ ] DP-13 — [Maximise cut segments](https://www.geeksforgeeks.org/problems/cutting-a-rod0416/1) — GFG practice
- [ ] DP-14 — [Longest common subsequence](https://www.geeksforgeeks.org/problems/longest-common-subsequence-1587115620/1) — GFG practice
- [ ] DP-15 — [Longest repeating subsequence](https://www.geeksforgeeks.org/problems/longest-repeating-subsequence/1) — GFG practice
- [ ] DP-16 — [Longest increasing subsequence](https://www.geeksforgeeks.org/problems/longest-increasing-subsequence-1587115620/1) — GFG practice
- [ ] DP-17 — [Space-optimised longest common subsequence](https://www.geeksforgeeks.org/space-optimized-solution-lcs/) — GFG article
- [ ] DP-18 — [Longest common subsequence of three strings](https://www.geeksforgeeks.org/problems/lcs-of-three-strings0028/1) — GFG practice
- [ ] DP-19 — [Maximum-sum increasing subsequence](https://www.geeksforgeeks.org/problems/maximum-sum-increasing-subsequence4749/1) — GFG practice
- [ ] DP-20 — [Count subsequences with product less than K](https://www.geeksforgeeks.org/count-subsequences-product-less-k/) — GFG article
- [ ] DP-21 — [Longest subsequence with adjacent difference one](https://www.geeksforgeeks.org/problems/longest-subsequence-1/1) — GFG practice
- [ ] DP-22 — [Maximum subsequence sum with no three consecutive elements](https://www.geeksforgeeks.org/maximum-subsequence-sum-such-that-no-three-are-consecutive/) — GFG article
- [ ] DP-23 — [Egg dropping](https://www.geeksforgeeks.org/problems/egg-dropping-puzzle-1587115620/1) — GFG practice
- [ ] DP-24 — [Maximum-length chain of pairs](https://www.geeksforgeeks.org/problems/max-length-chain/1) — GFG practice
- [ ] DP-25 — [Maximum square submatrix of 1s](https://www.geeksforgeeks.org/problems/largest-square-formed-in-a-matrix0806/1) — GFG practice
- [ ] DP-26 — [Maximum sum of pairs with a specific difference](https://www.geeksforgeeks.org/problems/maximum-sum-of-pairs-with-specific-difference1533/1) — GFG practice
- [ ] DP-27 — [Minimum-cost path](https://www.geeksforgeeks.org/min-cost-path-dp-6/) — GFG article
- [ ] DP-28 — [Maximum difference of zeros and ones in a binary string](https://www.geeksforgeeks.org/problems/maximum-difference-of-zeros-and-ones-in-binary-string4111/1) — GFG practice
- [ ] DP-29 — [Minimum jumps to reach the end](https://www.geeksforgeeks.org/problems/minimum-number-of-jumps/1) — GFG practice
- [ ] DP-30 — [Minimum cost to fill a bag of given weight](https://www.geeksforgeeks.org/problems/minimum-cost-to-fill-given-weight-in-a-bag1956/1) — GFG practice
- [ ] DP-31 — [Minimum removals so max - min <= K](https://www.geeksforgeeks.org/minimum-removals-array-make-max-min-k/) — GFG article
- [ ] DP-32 — [Longest common substring](https://www.geeksforgeeks.org/problems/longest-common-substring1452/1) — GFG practice
- [ ] DP-33 — [Number of ways to reach a game score](https://www.geeksforgeeks.org/problems/reach-a-given-score-1587115621/1) — GFG practice
- [ ] DP-34 — [Count balanced binary trees of height h](https://www.geeksforgeeks.org/problems/bt-with-factor-2/1) — GFG practice
- [ ] DP-35 — [Largest-sum contiguous subarray](https://www.geeksforgeeks.org/problems/kadanes-algorithm/1) — GFG practice
- [ ] DP-36 — [Smallest-sum contiguous subarray](https://www.geeksforgeeks.org/problems/smallest-sum-contiguous-subarray/1) — GFG practice
- [ ] DP-37 — [Unbounded knapsack](https://www.geeksforgeeks.org/problems/knapsack-with-duplicate-items4201/1) — GFG practice
- [ ] DP-38 — [Word break](https://www.geeksforgeeks.org/problems/word-break1352/1) — GFG practice
- [ ] DP-39 — [Largest independent set in a tree](https://www.geeksforgeeks.org/largest-independent-set-problem-using-dynamic-programming/) — GFG article
- [ ] DP-40 — [Equal-sum partition](https://www.geeksforgeeks.org/problems/subset-sum-problem2014/1) — GFG practice
- [ ] DP-41 — [Longest palindromic subsequence](https://www.geeksforgeeks.org/problems/longest-palindromic-subsequence-1612327878/1) — GFG practice
- [ ] DP-42 — [Count all palindromic subsequences](https://www.geeksforgeeks.org/problems/count-palindromic-subsequences/1) — GFG practice
- [ ] DP-43 — [Longest palindromic substring](https://www.geeksforgeeks.org/problems/longest-palindrome-in-a-string/1) — GFG practice
- [ ] DP-44 — [Longest alternating subsequence](https://www.geeksforgeeks.org/problems/longest-alternating-subsequence5951/1) — GFG practice
- [ ] DP-45 — [Weighted job scheduling](https://leetcode.com/problems/maximum-profit-in-job-scheduling/) — LeetCode
- [ ] DP-46 — [Coin game with three possible choices](https://www.geeksforgeeks.org/problems/coin-game-winner-where-every-player-has-three-choices-including-1/1) — GFG practice
- [ ] DP-47 — [Count derangements](https://www.geeksforgeeks.org/problems/dearrangement-of-balls0918/1) — GFG practice
- [ ] DP-48 — [Maximum stock profit with at most two transactions](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-iii/) — LeetCode
- [ ] DP-49 — [Optimal strategy for a game](https://www.geeksforgeeks.org/problems/optimal-strategy-for-a-game-1587115620/1) — GFG practice
- [ ] DP-50 — [Optimal binary search tree](https://www.geeksforgeeks.org/problems/optimal-binary-search-tree2214/1) — GFG practice
- [ ] DP-51 — [Palindrome partitioning: minimum cuts](https://www.geeksforgeeks.org/problems/palindromic-patitioning4845/1) — GFG practice
- [ ] DP-52 — [Word wrap](https://www.geeksforgeeks.org/problems/word-wrap1646/1) — GFG practice
- [ ] DP-53 — [Mobile numeric keypad](https://www.geeksforgeeks.org/problems/mobile-numeric-keypad5456/1) — GFG practice
- [ ] DP-54 — [Boolean parenthesisation](https://www.geeksforgeeks.org/problems/boolean-parenthesization5610/1) — GFG practice
- [ ] DP-55 — [Largest rectangular submatrix with sum zero](https://www.geeksforgeeks.org/largest-rectangular-sub-matrix-whose-sum-0/) — GFG article
- [ ] DP-56 — [Largest rectangular submatrix with equal 0s and 1s](https://www.geeksforgeeks.org/largest-area-rectangular-sub-matrix-equal-number-1s-0s/) — GFG article
- [ ] DP-57 — [Maximum-sum rectangle in a 2D matrix](https://www.geeksforgeeks.org/problems/maximum-sum-rectangle2948/1) — GFG practice
- [ ] DP-58 — [Maximum stock profit with at most K transactions](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-iv/) — LeetCode
- [ ] DP-59 — [Check whether a string is an interleaving of two others](https://leetcode.com/problems/interleaving-string/) — LeetCode
- [ ] DP-60 — [Maximum length of pair chain (retained repeated entry)](https://leetcode.com/problems/maximum-length-of-pair-chain/) — LeetCode

[Back to section counts](#section-navigation-and-counts)

## Bit Manipulation

10 entries.

- [ ] BIT-01 — [Count set bits in an integer](https://www.geeksforgeeks.org/problems/set-bits0143/1) — GFG practice
- [ ] BIT-02 — [Find two non-repeating elements](https://www.geeksforgeeks.org/problems/finding-the-numbers0215/1) — GFG practice
- [ ] BIT-03 — [Count bits to flip to convert A to B](https://www.geeksforgeeks.org/problems/bit-difference-1587115620/1) — GFG practice
- [ ] BIT-04 — [Total set bits in all numbers from 1 to n](https://www.geeksforgeeks.org/problems/count-total-set-bits-1587115620/1) — GFG practice
- [ ] BIT-05 — [Check whether a number is a power of two](https://www.geeksforgeeks.org/problems/power-of-2-1587115620/1) — GFG practice
- [ ] BIT-06 — [Position of the only set bit](https://www.geeksforgeeks.org/problems/find-position-of-set-bit3706/1) — GFG practice
- [ ] BIT-07 — [Copy set bits in a range](https://www.geeksforgeeks.org/copy-set-bits-in-a-range/) — GFG article
- [ ] BIT-08 — [Divide integers without multiplication, division or modulo](https://leetcode.com/problems/divide-two-integers/) — LeetCode
- [ ] BIT-09 — [Square a number without *, / or pow()](https://www.geeksforgeeks.org/calculate-square-of-a-number-without-using-and-pow/) — GFG article
- [ ] BIT-10 — [Power set](https://www.geeksforgeeks.org/problems/power-set4302/1) — GFG practice

[Back to section counts](#section-navigation-and-counts)

