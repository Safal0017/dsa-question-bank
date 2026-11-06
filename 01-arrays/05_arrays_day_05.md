# Arrays — Day 5

Love Babbar DSA Cracker Sheet  
Coverage: ARR-21 to ARR-25  
Questions: 5  
Examples: 3 per question  
Solutions and algorithm hints: intentionally omitted

## Today's questions

| ID | Problem | Practice |
| --- | --- | --- |
| ARR-21 | Detect a zero-sum subarray | [Practice](https://www.geeksforgeeks.org/problems/subarray-with-0-sum-1587115621/1) |
| ARR-22 | Factorial of a large number | [Practice](https://www.geeksforgeeks.org/problems/factorials-of-large-numbers2508/1) |
| ARR-23 | Maximum product subarray | [Practice](https://leetcode.com/problems/maximum-product-subarray/) |
| ARR-24 | Longest consecutive subsequence | [Practice](https://leetcode.com/problems/longest-consecutive-sequence/) |
| ARR-25 | Elements appearing more than n/k times | [Practice](https://www.geeksforgeeks.org/dsa/given-an-array-of-size-n-find-all-elements-that-appear-more-than-nk-times/) |

## Conventions

- Array displays describe function inputs and results, not stdin format.
- Examples are prepared for this pack; they are not necessarily platform examples.
- Rules below define the exact practice variant. Read any stated platform difference before submitting.
- Numeric platform limits are not reproduced here; consult the linked page for current judge constraints.
- Use a numeric type wide enough for the required sums, counts, and products.
- No solutions or algorithm steps are included.

---

## ARR-21 — Detect a zero-sum subarray

Practice: [Open problem](https://www.geeksforgeeks.org/problems/subarray-with-0-sum-1587115621/1)

### Problem statement

Given a non-empty integer array arr, return whether any non-empty contiguous subarray has sum zero.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

Return true or false. Negative values and zero are allowed. A subsequence with gaps does not qualify.

### Example 1

~~~text
Input:
arr = [4, 2, -3, 1, 6]

Expected result:
true
~~~

Explanation: [2, -3, 1] sums to zero.

### Example 2

~~~text
Input:
arr = [1, 2, 3]

Expected result:
false
~~~

Explanation: Every non-empty subarray has positive sum.

### Example 3

~~~text
Input:
arr = [0]

Expected result:
true
~~~

Explanation: The single-element subarray has sum zero.

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

## ARR-22 — Factorial of a large number

Practice: [Open problem](https://www.geeksforgeeks.org/problems/factorials-of-large-numbers2508/1)

### Problem statement

Given a non-negative integer n, return the decimal digits of n! in most-significant-first order.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

Use 0! = 1. Return a list of individual digits, not a fixed-width integer. Do not use BigInteger or another arbitrary-precision integer type for this practice exercise. Treat n up to 1000 as the practice range.

### Example 1

~~~text
Input:
n = 5

Expected result:
[1, 2, 0]
~~~

Explanation: 5! = 120.

### Example 2

~~~text
Input:
n = 10

Expected result:
[3, 6, 2, 8, 8, 0, 0]
~~~

Explanation: 10! = 3628800.

### Example 3

~~~text
Input:
n = 0

Expected result:
[1]
~~~

Explanation: Zero factorial is one.

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

## ARR-23 — Maximum product subarray

Practice: [Open problem](https://leetcode.com/problems/maximum-product-subarray/)

### Problem statement

Given a non-empty integer array arr, return the largest product of a non-empty contiguous subarray.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

Values can be positive, negative, or zero. A subarray must be contiguous. For this practice pack, assume the product of any subarray fits in a signed 32-bit integer.

### Example 1

~~~text
Input:
arr = [2, 3, -2, 4]

Expected result:
6
~~~

Explanation: [2, 3] has product 6.

### Example 2

~~~text
Input:
arr = [-2, 0, -1]

Expected result:
0
~~~

Explanation: [-2, -1] is not contiguous in this input.

### Example 3

~~~text
Input:
arr = [-2, 3, -4]

Expected result:
24
~~~

Explanation: The entire array has product 24.

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

## ARR-24 — Longest consecutive subsequence

Practice: [Open problem](https://leetcode.com/problems/longest-consecutive-sequence/)

### Problem statement

Given an integer array arr, return the length of the longest sequence of distinct consecutive integer values present in it.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

The input is unsorted. Values need not occupy adjacent indices or appear in increasing input order. Duplicates do not increase the length. Return zero for an empty array. The linked judge requests O(n) time.

### Example 1

~~~text
Input:
arr = [100, 4, 200, 1, 3, 2]

Expected result:
4
~~~

Explanation: The values 1, 2, 3, 4 are present.

### Example 2

~~~text
Input:
arr = [1, 2, 2, 3]

Expected result:
3
~~~

Explanation: The repeated 2 does not extend the sequence.

### Example 3

~~~text
Input:
arr = []

Expected result:
0
~~~

Explanation: No values are present.

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

## ARR-25 — Elements appearing more than n/k times

Practice: [Open problem](https://www.geeksforgeeks.org/dsa/given-an-array-of-size-n-find-all-elements-that-appear-more-than-nk-times/)

### Problem statement

Given a non-empty integer array arr of length n and an integer k >= 2, return every distinct value whose frequency is strictly greater than n/k.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

Compare against the mathematical ratio n/k. Return values sorted in increasing order for a deterministic result. Return an empty list if none qualifies. This exercise asks for the values, not just their count.

### Example 1

~~~text
Input:
arr = [3, 1, 2, 2, 1, 2, 3, 3]; k = 4

Expected result:
[2, 3]
~~~

Explanation: n/k is 2; each returned value occurs three times.

### Example 2

~~~text
Input:
arr = [1, 1, 2, 2]; k = 2

Expected result:
[]
~~~

Explanation: Each frequency equals 2, but must be strictly greater than 2.

### Example 3

~~~text
Input:
arr = [5, 5, 5, 2]; k = 3

Expected result:
[5]
~~~

Explanation: 3 is greater than 4/3; 1 is not.

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

## Day 5 review

| ID | Understood | Implemented | Validated | Complexity explained | Revisit |
| --- | --- | --- | --- | --- | --- |
| ARR-21 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-22 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-23 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-24 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-25 | [ ] | [ ] | [ ] | [ ] | [ ] |
