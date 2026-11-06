# Arrays — Day 2

Love Babbar DSA Cracker Sheet  
Coverage: ARR-06 to ARR-10  
Questions: 5  
Examples: 3 per question  
Solutions and algorithm hints: intentionally omitted

## Today's questions

| ID | Problem | Practice |
| --- | --- | --- |
| ARR-06 | Union and intersection of two sorted arrays | [Practice](https://www.geeksforgeeks.org/problems/union-of-two-sorted-arrays-1587115621/1) |
| ARR-07 | Cyclically rotate an array by one | [Practice](https://www.geeksforgeeks.org/problems/cyclically-rotate-an-array-by-one2614/1) |
| ARR-08 | Largest sum contiguous subarray | [Practice](https://leetcode.com/problems/maximum-subarray/) |
| ARR-09 | Minimize the maximum difference between heights | [Practice](https://www.geeksforgeeks.org/problems/minimize-the-heights3351/1) |
| ARR-10 | Minimum jumps to reach the end | [Practice](https://www.geeksforgeeks.org/problems/minimum-number-of-jumps-1587115620/1) |

## Conventions

- Array displays describe function inputs and results, not stdin format.
- Examples are prepared for this pack; they are not necessarily platform examples.
- Rules below define the exact practice variant. Read any stated platform difference before submitting.
- Numeric platform limits are not reproduced here; consult the linked page for current judge constraints.
- Use a numeric type wide enough for the required sums, counts, and products.
- No solutions or algorithm steps are included.

---

## ARR-06 — Union and intersection of two sorted arrays

Practice: [Open problem](https://www.geeksforgeeks.org/problems/union-of-two-sorted-arrays-1587115621/1)

### Problem statement

Given two non-empty arrays a and b sorted in non-decreasing order, return their union and intersection as two sorted arrays. Include each distinct value only once in each result.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

Return [union, intersection]. Duplicates do not create repeated output values. Solve both parts; the linked judge covers the union part. Inputs may have different lengths.

### Example 1

~~~text
Input:
a = [1, 2, 2, 4]; b = [2, 3, 4]

Expected result:
[[1, 2, 3, 4], [2, 4]]
~~~

Explanation: The common distinct values are 2 and 4.

### Example 2

~~~text
Input:
a = [1, 1]; b = [2, 2]

Expected result:
[[1, 2], []]
~~~

Explanation: No value occurs in both arrays.

### Example 3

~~~text
Input:
a = [5]; b = [5]

Expected result:
[[5], [5]]
~~~

Explanation: The repeated value appears once in each result.

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

## ARR-07 — Cyclically rotate an array by one

Practice: [Open problem](https://www.geeksforgeeks.org/problems/cyclically-rotate-an-array-by-one2614/1)

### Problem statement

Given a non-empty integer array arr, rotate it right by exactly one position. Update the supplied array.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

The last element becomes the first. All other elements move one position right. This is not reversal.

### Example 1

~~~text
Input:
arr = [1, 2, 3, 4, 5]

Expected result:
[5, 1, 2, 3, 4]
~~~

Explanation: 5 moves to the front.

### Example 2

~~~text
Input:
arr = [8, 8, 2]

Expected result:
[2, 8, 8]
~~~

Explanation: Both occurrences of 8 remain.

### Example 3

~~~text
Input:
arr = [7]

Expected result:
[7]
~~~

Explanation: A single-element array remains unchanged.

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

## ARR-08 — Largest sum contiguous subarray

Practice: [Open problem](https://leetcode.com/problems/maximum-subarray/)

### Problem statement

Given a non-empty integer array arr, return the largest sum obtainable from a non-empty contiguous subarray.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

Return the sum, not the subarray or its indices. Negative values are allowed. An empty subarray with sum zero is not permitted. ARR-13 is a separate sheet entry for the same underlying problem.

### Example 1

~~~text
Input:
arr = [-2, 1, -3, 4, -1, 2, 1, -5, 4]

Expected result:
6
~~~

Explanation: [4, -1, 2, 1] has sum 6.

### Example 2

~~~text
Input:
arr = [-8, -3, -6]

Expected result:
-3
~~~

Explanation: The single element -3 is the best non-empty choice.

### Example 3

~~~text
Input:
arr = [5]

Expected result:
5
~~~

Explanation: The only subarray contains 5.

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

## ARR-09 — Minimize the maximum difference between heights

Practice: [Open problem](https://www.geeksforgeeks.org/problems/minimize-the-heights3351/1)

### Problem statement

Given non-negative tower heights arr and a positive integer k, change every height by either +k or -k exactly once. Return the minimum possible difference between the largest and smallest resulting heights.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

Every tower must change. No resulting height may be negative. This pack uses the Minimize the Heights II variant, not a variant allowing negative heights.

### Example 1

~~~text
Input:
arr = [1, 5, 8, 10]; k = 2

Expected result:
5
~~~

Explanation: [3, 3, 6, 8] is a valid optimal result.

### Example 2

~~~text
Input:
arr = [3, 9, 12, 16, 20]; k = 3

Expected result:
11
~~~

Explanation: [6, 12, 9, 13, 17] has range 11.

### Example 3

~~~text
Input:
arr = [4]; k = 5

Expected result:
0
~~~

Explanation: The only valid final height is 9; a single height has range zero.

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

## ARR-10 — Minimum jumps to reach the end

Practice: [Open problem](https://www.geeksforgeeks.org/problems/minimum-number-of-jumps-1587115620/1)

### Problem statement

Given a non-empty array arr of non-negative integers, start at index 0. From index i, you may jump forward by any positive distance at most arr[i]. Return the minimum jumps needed to reach the last index, or -1 if impossible.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

A value is a maximum jump length, not a required jump length. A single-element array needs zero jumps. Do not jump outside the array.

### Example 1

~~~text
Input:
arr = [2, 3, 1, 1, 4]

Expected result:
2
~~~

Explanation: Indices 0 -> 1 -> 4 reach the end in two jumps.

### Example 2

~~~text
Input:
arr = [1, 0, 2]

Expected result:
-1
~~~

Explanation: You become stuck at index 1.

### Example 3

~~~text
Input:
arr = [0]

Expected result:
0
~~~

Explanation: The starting index is already the destination.

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

## Day 2 review

| ID | Understood | Implemented | Validated | Complexity explained | Revisit |
| --- | --- | --- | --- | --- | --- |
| ARR-06 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-07 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-08 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-09 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-10 | [ ] | [ ] | [ ] | [ ] | [ ] |
