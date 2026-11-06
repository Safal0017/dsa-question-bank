# Arrays — Day 4

Love Babbar DSA Cracker Sheet  
Coverage: ARR-16 to ARR-20  
Questions: 5  
Examples: 3 per question  
Solutions and algorithm hints: intentionally omitted

## Today's questions

| ID | Problem | Practice |
| --- | --- | --- |
| ARR-16 | Count inversions | [Practice](https://www.geeksforgeeks.org/problems/inversion-of-array-1587115620/1) |
| ARR-17 | Best time to buy and sell stock — one transaction | [Practice](https://leetcode.com/problems/best-time-to-buy-and-sell-stock/) |
| ARR-18 | Count pairs with a given sum | [Practice](https://www.geeksforgeeks.org/problems/count-pairs-with-given-sum5022/1) |
| ARR-19 | Common elements in three sorted arrays | [Practice](https://www.geeksforgeeks.org/problems/common-elements1132/1) |
| ARR-20 | Rearrange alternating positive and negative elements | [Practice](https://www.geeksforgeeks.org/dsa/rearrange-array-alternating-positive-negative-items-o1-extra-space/) |

## Conventions

- Array displays describe function inputs and results, not stdin format.
- Examples are prepared for this pack; they are not necessarily platform examples.
- Rules below define the exact practice variant. Read any stated platform difference before submitting.
- Numeric platform limits are not reproduced here; consult the linked page for current judge constraints.
- Use a numeric type wide enough for the required sums, counts, and products.
- No solutions or algorithm steps are included.

---

## ARR-16 — Count inversions

Practice: [Open problem](https://www.geeksforgeeks.org/problems/inversion-of-array-1587115620/1)

### Problem statement

Given a non-empty integer array arr, count pairs of indices (i, j) such that i < j and arr[i] > arr[j].

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

Return the number of index pairs, not distinct value pairs. Equal values do not form an inversion. Use a return type large enough for n * (n - 1) / 2.

### Example 1

~~~text
Input:
arr = [2, 4, 1, 3, 5]

Expected result:
3
~~~

Explanation: The inverted value pairs are (2, 1), (4, 1), and (4, 3).

### Example 2

~~~text
Input:
arr = [3, 2, 1]

Expected result:
3
~~~

Explanation: Every index pair is inverted.

### Example 3

~~~text
Input:
arr = [1, 1, 1]

Expected result:
0
~~~

Explanation: Equal values do not qualify.

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

## ARR-17 — Best time to buy and sell stock — one transaction

Practice: [Open problem](https://leetcode.com/problems/best-time-to-buy-and-sell-stock/)

### Problem statement

Given a non-empty array prices where prices[i] is the price on day i, return the maximum profit from at most one buy followed by one sale on a later day.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

You may choose not to trade, giving profit zero. You cannot sell before buying or hold multiple shares. Prices are non-negative.

### Example 1

~~~text
Input:
prices = [7, 1, 5, 3, 6, 4]

Expected result:
5
~~~

Explanation: Buy at 1 and later sell at 6.

### Example 2

~~~text
Input:
prices = [7, 6, 4, 3, 1]

Expected result:
0
~~~

Explanation: No profitable transaction exists.

### Example 3

~~~text
Input:
prices = [2]

Expected result:
0
~~~

Explanation: There is no later day on which to sell.

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

## ARR-18 — Count pairs with a given sum

Practice: [Open problem](https://www.geeksforgeeks.org/problems/count-pairs-with-given-sum5022/1)

### Problem statement

Given an integer array arr and integer target, return the number of index pairs (i, j) with i < j and arr[i] + arr[j] = target.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

This pack uses the pair-count variant. Different index pairs count separately even when their values match. Do not reuse one index within a pair. The sheet wording says find all pairs; this exercise requests their count.

### Example 1

~~~text
Input:
arr = [1, 5, 7, -1, 5]; target = 6

Expected result:
3
~~~

Explanation: Pairs by index are (0,1), (0,4), and (2,3).

### Example 2

~~~text
Input:
arr = [1, 1, 1, 1]; target = 2

Expected result:
6
~~~

Explanation: All six distinct index pairs qualify.

### Example 3

~~~text
Input:
arr = [2, 4, 6]; target = 5

Expected result:
0
~~~

Explanation: No pair has the target sum.

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

## ARR-19 — Common elements in three sorted arrays

Practice: [Open problem](https://www.geeksforgeeks.org/problems/common-elements1132/1)

### Problem statement

Given three non-empty arrays a, b, and c sorted in non-decreasing order, return the distinct values present in all three, in increasing order.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

Repeated occurrences do not repeat the output value. Return an empty list when there is no common value; if a judge uses a display sentinel, follow its driver format.

### Example 1

~~~text
Input:
a = [1, 5, 10, 20, 40, 80]; b = [6, 7, 20, 80, 100]; c = [3, 4, 15, 20, 30, 70, 80, 120]

Expected result:
[20, 80]
~~~

Explanation: Both values occur in every array.

### Example 2

~~~text
Input:
a = [1, 1, 2]; b = [1, 1]; c = [1, 3]

Expected result:
[1]
~~~

Explanation: Return 1 once.

### Example 3

~~~text
Input:
a = [1]; b = [2]; c = [3]

Expected result:
[]
~~~

Explanation: There is no value shared by all three.

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

## ARR-20 — Rearrange alternating positive and negative elements

Practice: [Open problem](https://www.geeksforgeeks.org/dsa/rearrange-array-alternating-positive-negative-items-o1-extra-space/)

### Problem statement

Rearrange arr so non-negative and negative values alternate, beginning with a non-negative value where possible. Preserve relative order within both groups. Append the remaining group when the other runs out.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

For this pack, zero belongs to the non-negative group. Update arr using O(1) auxiliary space. If no non-negative value exists, leave the negative sequence unchanged. Unequal group sizes are allowed. This is the stable, unequal-count variant, not the equal-count LeetCode problem.

### Example 1

~~~text
Input:
arr = [-1, 2, -3, 4, 5, -6]

Expected result:
[2, -1, 4, -3, 5, -6]
~~~

Explanation: Both groups preserve their original order.

### Example 2

~~~text
Input:
arr = [1, 2, 3, -4]

Expected result:
[1, -4, 2, 3]
~~~

Explanation: The unused non-negative values form the suffix.

### Example 3

~~~text
Input:
arr = [-2, 0, -1, -3]

Expected result:
[0, -2, -1, -3]
~~~

Explanation: Zero starts the sequence; the remaining negatives keep their order.

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

## Day 4 review

| ID | Understood | Implemented | Validated | Complexity explained | Revisit |
| --- | --- | --- | --- | --- | --- |
| ARR-16 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-17 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-18 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-19 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-20 | [ ] | [ ] | [ ] | [ ] | [ ] |
