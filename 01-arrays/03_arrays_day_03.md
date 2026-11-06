# Arrays — Day 3

Love Babbar DSA Cracker Sheet  
Coverage: ARR-11 to ARR-15  
Questions: 5  
Examples: 3 per question  
Solutions and algorithm hints: intentionally omitted

## Today's questions

| ID | Problem | Practice |
| --- | --- | --- |
| ARR-11 | Find the duplicate number | [Practice](https://leetcode.com/problems/find-the-duplicate-number/) |
| ARR-12 | Merge two sorted arrays without extra space | [Practice](https://www.geeksforgeeks.org/problems/merge-two-sorted-arrays-1587115620/1) |
| ARR-13 | Maximum subarray sum — repeated sheet entry | [Practice](https://leetcode.com/problems/maximum-subarray/) |
| ARR-14 | Merge overlapping intervals | [Practice](https://leetcode.com/problems/merge-intervals/) |
| ARR-15 | Next permutation | [Practice](https://leetcode.com/problems/next-permutation/) |

## Conventions

- Array displays describe function inputs and results, not stdin format.
- Examples are prepared for this pack; they are not necessarily platform examples.
- Rules below define the exact practice variant. Read any stated platform difference before submitting.
- Numeric platform limits are not reproduced here; consult the linked page for current judge constraints.
- Use a numeric type wide enough for the required sums, counts, and products.
- No solutions or algorithm steps are included.

---

## ARR-11 — Find the duplicate number

Practice: [Open problem](https://leetcode.com/problems/find-the-duplicate-number/)

### Problem statement

Given n + 1 integers in arr, where every value is in [1, n], return the one value that appears more than once.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

Exactly one distinct value repeats; it may appear more than twice. Do not modify arr. Use constant auxiliary space. These requirements follow the linked LeetCode variant.

### Example 1

~~~text
Input:
arr = [1, 3, 4, 2, 2]

Expected result:
2
~~~

Explanation: 2 occurs twice.

### Example 2

~~~text
Input:
arr = [3, 1, 3, 4, 2]

Expected result:
3
~~~

Explanation: 3 is the repeated value.

### Example 3

~~~text
Input:
arr = [2, 2, 2, 2, 2]

Expected result:
2
~~~

Explanation: Only one distinct value repeats, even though it occurs five times.

### My working area

- Straightforward approach:
- Improved approach:
- Time complexity:
- Auxiliary-space complexity:
- Additional tests:
- Mistakes or observations:

- [ ] Implemented
- [ ] All three examples passed
- [ ] Additional edge cases passed
- [ ] Can explain correctness and complexity

---

## ARR-12 — Merge two sorted arrays without extra space

Practice: [Open problem](https://www.geeksforgeeks.org/problems/merge-two-sorted-arrays-1587115620/1)

### Problem statement

Given non-empty sorted arrays a and b of lengths n and m, rearrange their values so a contains the smallest n values and b contains the remaining m values. Both arrays must remain sorted.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

Update both arrays in place. Their lengths do not change. Use O(1) auxiliary space; do not create a third array. This is not the padded-array LeetCode merge variant.

### Example 1

~~~text
Input:
a = [1, 4, 7, 8, 10]; b = [2, 3, 9]

Expected result:
a = [1, 2, 3, 4, 7]; b = [8, 9, 10]
~~~

Explanation: The first array retains five positions.

### Example 2

~~~text
Input:
a = [1, 2]; b = [3, 4]

Expected result:
a = [1, 2]; b = [3, 4]
~~~

Explanation: The arrays already satisfy the requirement.

### Example 3

~~~text
Input:
a = [5]; b = [1, 2]

Expected result:
a = [1]; b = [2, 5]
~~~

Explanation: The smallest value belongs in a.

### My working area

- Straightforward approach:
- Improved approach:
- Time complexity:
- Auxiliary-space complexity:
- Additional tests:
- Mistakes or observations:

- [ ] Implemented
- [ ] All three examples passed
- [ ] Additional edge cases passed
- [ ] Can explain correctness and complexity

---

## ARR-13 — Maximum subarray sum — repeated sheet entry

Practice: [Open problem](https://leetcode.com/problems/maximum-subarray/)

### Problem statement

Given a non-empty integer array arr, return the maximum sum of a non-empty contiguous subarray.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

This is the sheet entry titled Kadane's Algo. Its title names a technique, but no solution steps are supplied here. ARR-08 and ARR-13 remain separate to preserve all 36 sheet entries. Attempt this again independently.

### Example 1

~~~text
Input:
arr = [1, 2, 3, -2, 5]

Expected result:
9
~~~

Explanation: The entire array sums to 9.

### Example 2

~~~text
Input:
arr = [-4, -1, -7]

Expected result:
-1
~~~

Explanation: Choosing an empty subarray is not allowed.

### Example 3

~~~text
Input:
arr = [0, -2, 0]

Expected result:
0
~~~

Explanation: A single zero is a valid best subarray.

### My working area

- Straightforward approach:
- Improved approach:
- Time complexity:
- Auxiliary-space complexity:
- Additional tests:
- Mistakes or observations:

- [ ] Implemented
- [ ] All three examples passed
- [ ] Additional edge cases passed
- [ ] Can explain correctness and complexity

---

## ARR-14 — Merge overlapping intervals

Practice: [Open problem](https://leetcode.com/problems/merge-intervals/)

### Problem statement

Given a non-empty list of closed intervals [start, end], merge every overlapping group and return the resulting non-overlapping intervals sorted by start.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

Each start is at most its end. Intervals sharing an endpoint overlap. The original intervals need not be sorted.

### Example 1

~~~text
Input:
intervals = [[1, 3], [2, 6], [8, 10], [15, 18]]

Expected result:
[[1, 6], [8, 10], [15, 18]]
~~~

Explanation: The first two intervals overlap.

### Example 2

~~~text
Input:
intervals = [[1, 4], [4, 5]]

Expected result:
[[1, 5]]
~~~

Explanation: The shared endpoint 4 makes them overlap.

### Example 3

~~~text
Input:
intervals = [[1, 10], [2, 3], [4, 8]]

Expected result:
[[1, 10]]
~~~

Explanation: Both smaller intervals are contained in the first.

### My working area

- Straightforward approach:
- Improved approach:
- Time complexity:
- Auxiliary-space complexity:
- Additional tests:
- Mistakes or observations:

- [ ] Implemented
- [ ] All three examples passed
- [ ] Additional edge cases passed
- [ ] Can explain correctness and complexity

---

## ARR-15 — Next permutation

Practice: [Open problem](https://leetcode.com/problems/next-permutation/)

### Problem statement

Given a non-empty integer array arr, rearrange it into the next lexicographically greater permutation. If none exists, rearrange it into the smallest possible permutation.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

Update arr in place using constant auxiliary space. Duplicate values are allowed. Compare permutations from left to right at the first differing position.

### Example 1

~~~text
Input:
arr = [1, 2, 3]

Expected result:
[1, 3, 2]
~~~

Explanation: This is the next greater ordering.

### Example 2

~~~text
Input:
arr = [3, 2, 1]

Expected result:
[1, 2, 3]
~~~

Explanation: No greater ordering exists, so wrap to the smallest.

### Example 3

~~~text
Input:
arr = [1, 1, 5]

Expected result:
[1, 5, 1]
~~~

Explanation: Repeated values are not distinct labels.

### My working area

- Straightforward approach:
- Improved approach:
- Time complexity:
- Auxiliary-space complexity:
- Additional tests:
- Mistakes or observations:

- [ ] Implemented
- [ ] All three examples passed
- [ ] Additional edge cases passed
- [ ] Can explain correctness and complexity

---

## Day 3 review

| ID | Understood | Implemented | Validated | Complexity explained | Revisit |
| --- | --- | --- | --- | --- | --- |
| ARR-11 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-12 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-13 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-14 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-15 | [ ] | [ ] | [ ] | [ ] | [ ] |
