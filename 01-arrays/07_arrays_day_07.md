# Arrays — Day 7

Love Babbar DSA Cracker Sheet  
Coverage: ARR-31 to ARR-36  
Questions: 6  
Examples: 3 per question  
Solutions and algorithm hints: intentionally omitted

## Today's questions

| ID | Problem | Practice |
| --- | --- | --- |
| ARR-31 | Smallest subarray with sum strictly greater than x | [Practice](https://www.geeksforgeeks.org/problems/smallest-subarray-with-sum-greater-than-x4370/1) |
| ARR-32 | Three-way partition around a range | [Practice](https://www.geeksforgeeks.org/problems/three-way-partitioning/1) |
| ARR-33 | Minimum swaps to bring values at most k together | [Practice](https://www.geeksforgeeks.org/problems/minimum-swaps-required-to-bring-all-elements-less-than-or-equal-to-k-together/1) |
| ARR-34 | Minimum merge operations to make an array palindromic | [Practice](https://www.geeksforgeeks.org/dsa/find-minimum-number-of-merge-operations-to-make-an-array-palindrome/) |
| ARR-35 | Median of two sorted arrays of equal size | [Practice](https://leetcode.com/problems/median-of-two-sorted-arrays/) |
| ARR-36 | Median of two sorted arrays of different sizes | [Practice](https://leetcode.com/problems/median-of-two-sorted-arrays/) |

## Conventions

- Array displays describe function inputs and results, not stdin format.
- Examples are prepared for this pack; they are not necessarily platform examples.
- Rules below define the exact practice variant. Read any stated platform difference before submitting.
- Numeric platform limits are not reproduced here; consult the linked page for current judge constraints.
- Use a numeric type wide enough for the required sums, counts, and products.
- No solutions or algorithm steps are included.

---

## ARR-31 — Smallest subarray with sum strictly greater than x

Practice: [Open problem](https://www.geeksforgeeks.org/problems/smallest-subarray-with-sum-greater-than-x4370/1)

### Problem statement

Given a non-empty array arr of non-negative integers and a non-negative integer x, return the minimum length of a contiguous subarray whose sum is strictly greater than x. Return 0 if none exists.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

Equality with x is insufficient. Negative elements are outside this variant. Return the length, not the sum or indices.

### Example 1

~~~text
Input:
arr = [1, 4, 45, 6, 0, 19]; x = 51

Expected result:
3
~~~

Explanation: [4, 45, 6] sums to 55; [45, 6] only equals 51.

### Example 2

~~~text
Input:
arr = [1, 2, 3]; x = 6

Expected result:
0
~~~

Explanation: Even the full array only equals 6.

### Example 3

~~~text
Input:
arr = [0, 0, 5]; x = 0

Expected result:
1
~~~

Explanation: [5] is a qualifying one-element subarray.

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

## ARR-32 — Three-way partition around a range

Practice: [Open problem](https://www.geeksforgeeks.org/problems/three-way-partitioning/1)

### Problem statement

Given an integer array arr and bounds a <= b, rearrange arr into three consecutive groups: values less than a, values in [a, b], and values greater than b.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

Update arr in place using O(1) auxiliary space. Preserve all occurrences. Internal ordering within each group is unrestricted. Displayed outputs are examples, not unique answers.

### Example 1

~~~text
Input:
arr = [1, 2, 3, 3, 4]; a = 1; b = 2

Expected result:
One valid array: [1, 2, 3, 3, 4]
~~~

Explanation: The less-than-a group is empty.

### Example 2

~~~text
Input:
arr = [4, 1, 7, 3, 2, 6]; a = 2; b = 4

Expected result:
One valid array: [1, 4, 3, 2, 7, 6]
~~~

Explanation: The groups are [1], [4,3,2], and [7,6].

### Example 3

~~~text
Input:
arr = [5, 5, 5]; a = 5; b = 5

Expected result:
One valid array: [5, 5, 5]
~~~

Explanation: Every value belongs to the middle group.

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

## ARR-33 — Minimum swaps to bring values at most k together

Practice: [Open problem](https://www.geeksforgeeks.org/problems/minimum-swaps-required-to-bring-all-elements-less-than-or-equal-to-k-together/1)

### Problem statement

Given a non-empty integer array arr and integer k, return the minimum swaps required to make all values <= k occupy one contiguous block.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

One swap may exchange any two indices; it is not restricted to adjacent positions. The block may appear anywhere. Its internal order does not matter. If zero or one value qualifies, return zero.

### Example 1

~~~text
Input:
arr = [2, 1, 5, 6, 3]; k = 3

Expected result:
1
~~~

Explanation: Swap 5 and 3 to obtain [2, 1, 3, 6, 5].

### Example 2

~~~text
Input:
arr = [1, 2, 3, 9]; k = 3

Expected result:
0
~~~

Explanation: The qualifying values already form a block.

### Example 3

~~~text
Input:
arr = [7, 8, 9]; k = 3

Expected result:
0
~~~

Explanation: No values need to be grouped.

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

## ARR-34 — Minimum merge operations to make an array palindromic

Practice: [Open problem](https://www.geeksforgeeks.org/dsa/find-minimum-number-of-merge-operations-to-make-an-array-palindrome/)

### Problem statement

Given a non-empty array arr of positive integers, return the minimum operations needed to make its sequence palindromic. In one operation, replace two adjacent values by their sum, reducing the length by one.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

Only adjacent merges are allowed. This is not arbitrary replacement, deletion, or swapping. A single-element sequence is a palindrome. Original values are strictly positive.

### Example 1

~~~text
Input:
arr = [1, 4, 5, 1]

Expected result:
1
~~~

Explanation: Merge 4 and 5 to obtain [1, 9, 1].

### Example 2

~~~text
Input:
arr = [1, 2, 3]

Expected result:
1
~~~

Explanation: Merge 1 and 2 to obtain [3, 3].

### Example 3

~~~text
Input:
arr = [1, 2, 2, 1]

Expected result:
0
~~~

Explanation: The sequence is already palindromic.

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

## ARR-35 — Median of two sorted arrays of equal size

Practice: [Open problem](https://leetcode.com/problems/median-of-two-sorted-arrays/)

### Problem statement

Given two non-empty sorted integer arrays a and b of the same length n, return the median of their combined 2n values.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

This is the equal-size restriction of the linked general problem. Count duplicates separately. Since the total length is even, return the average of the two middle values as a number that can represent fractions. The linked judge requests O(log(m+n)) time.

### Example 1

~~~text
Input:
a = [1, 12, 15, 26, 38]; b = [2, 13, 17, 30, 45]

Expected result:
16.0
~~~

Explanation: The middle values are 15 and 17.

### Example 2

~~~text
Input:
a = [1]; b = [2]

Expected result:
1.5
~~~

Explanation: The median is (1 + 2) / 2.

### Example 3

~~~text
Input:
a = [0, 0]; b = [0, 0]

Expected result:
0.0
~~~

Explanation: Every combined value is zero.

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

## ARR-36 — Median of two sorted arrays of different sizes

Practice: [Open problem](https://leetcode.com/problems/median-of-two-sorted-arrays/)

### Problem statement

Given sorted integer arrays a and b of lengths m and n, return the median of their combined values. Their sizes need not match.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

Either array may be empty, but m + n must be positive. For an odd total length, return the middle value; for an even total, average the two middle values. Duplicates count separately. The linked judge requests O(log(m+n)) time.

### Example 1

~~~text
Input:
a = [1, 3]; b = [2]

Expected result:
2.0
~~~

Explanation: The combined ordering is [1, 2, 3].

### Example 2

~~~text
Input:
a = [1, 2]; b = [3, 4, 5, 6]

Expected result:
3.5
~~~

Explanation: The two middle values are 3 and 4.

### Example 3

~~~text
Input:
a = []; b = [7]

Expected result:
7.0
~~~

Explanation: The sole combined value is 7.

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

## Day 7 review

| ID | Understood | Implemented | Validated | Complexity explained | Revisit |
| --- | --- | --- | --- | --- | --- |
| ARR-31 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-32 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-33 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-34 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-35 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-36 | [ ] | [ ] | [ ] | [ ] | [ ] |
