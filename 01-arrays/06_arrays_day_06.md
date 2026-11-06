# Arrays — Day 6

Love Babbar DSA Cracker Sheet  
Coverage: ARR-26 to ARR-30  
Questions: 5  
Examples: 3 per question  
Solutions and algorithm hints: intentionally omitted

## Today's questions

| ID | Problem | Practice |
| --- | --- | --- |
| ARR-26 | Stock profit with at most two transactions | [Practice](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-iii/) |
| ARR-27 | Check whether one array is a subset of another | [Practice](https://www.geeksforgeeks.org/problems/array-subset-of-another-array2317/1) |
| ARR-28 | Find whether a triplet has a given sum | [Practice](https://www.geeksforgeeks.org/problems/triplet-sum-in-array-1587115621/1) |
| ARR-29 | Trapping rain water | [Practice](https://leetcode.com/problems/trapping-rain-water/) |
| ARR-30 | Chocolate distribution | [Practice](https://www.geeksforgeeks.org/problems/chocolate-distribution-problem3825/1) |

## Conventions

- Array displays describe function inputs and results, not stdin format.
- Examples are prepared for this pack; they are not necessarily platform examples.
- Rules below define the exact practice variant. Read any stated platform difference before submitting.
- Numeric platform limits are not reproduced here; consult the linked page for current judge constraints.
- Use a numeric type wide enough for the required sums, counts, and products.
- No solutions or algorithm steps are included.

---

## ARR-26 — Stock profit with at most two transactions

Practice: [Open problem](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-iii/)

### Problem statement

Given a non-empty array of non-negative stock prices, return the maximum profit from at most two buy-then-sell transactions.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

Complete one transaction before starting the next. Hold at most one share. Zero or one transaction is allowed. This is not the unlimited-transactions variant.

### Example 1

~~~text
Input:
prices = [3, 3, 5, 0, 0, 3, 1, 4]

Expected result:
6
~~~

Explanation: Buy at 0 and sell at 3, then buy at 1 and sell at 4.

### Example 2

~~~text
Input:
prices = [1, 2, 3, 4, 5]

Expected result:
4
~~~

Explanation: One transaction from 1 to 5 is enough.

### Example 3

~~~text
Input:
prices = [7, 6, 4, 3, 1]

Expected result:
0
~~~

Explanation: Skipping all trades is best.

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

## ARR-27 — Check whether one array is a subset of another

Practice: [Open problem](https://www.geeksforgeeks.org/problems/array-subset-of-another-array2317/1)

### Problem statement

Given arrays a and b, return whether every occurrence in b can be matched to a distinct occurrence with the same value in a.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

This pack uses multiset inclusion: frequencies matter. The arrays are not guaranteed to be sorted. An empty b is a subset of every a.

### Example 1

~~~text
Input:
a = [1, 2, 2, 3]; b = [2, 2]

Expected result:
true
~~~

Explanation: a contains two occurrences of 2.

### Example 2

~~~text
Input:
a = [1, 2, 3]; b = [2, 2]

Expected result:
false
~~~

Explanation: a has only one occurrence of 2.

### Example 3

~~~text
Input:
a = [4, 5]; b = []

Expected result:
true
~~~

Explanation: There is nothing to match.

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

## ARR-28 — Find whether a triplet has a given sum

Practice: [Open problem](https://www.geeksforgeeks.org/problems/triplet-sum-in-array-1587115621/1)

### Problem statement

Given an integer array arr and integer target, return whether three distinct indices have values summing to target.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

Return a boolean, not all triplets. Equal values may be used if they occur at different indices. Fewer than three elements means false.

### Example 1

~~~text
Input:
arr = [1, 4, 45, 6, 10, 8]; target = 22

Expected result:
true
~~~

Explanation: 4 + 10 + 8 = 22.

### Example 2

~~~text
Input:
arr = [2, 2, 2]; target = 6

Expected result:
true
~~~

Explanation: The three occurrences occupy distinct indices.

### Example 3

~~~text
Input:
arr = [1, 2, 3]; target = 10

Expected result:
false
~~~

Explanation: The only triplet sums to 6.

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

## ARR-29 — Trapping rain water

Practice: [Open problem](https://leetcode.com/problems/trapping-rain-water/)

### Problem statement

Given a non-empty array height of non-negative integers representing unit-width elevation bars, return the total units of rain water trapped after rainfall.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

Water must be bounded by bars on both sides. Return the total volume, not the tallest water level or the area of a container formed by two bars.

### Example 1

~~~text
Input:
height = [0, 1, 0, 2, 1, 0, 1, 3, 2, 1, 2, 1]

Expected result:
6
~~~

Explanation: The enclosed positions collectively hold six units.

### Example 2

~~~text
Input:
height = [4, 2, 0, 3, 2, 5]

Expected result:
9
~~~

Explanation: The interior positions hold 2, 4, 1, and 2 units.

### Example 3

~~~text
Input:
height = [1, 2, 3]

Expected result:
0
~~~

Explanation: There is no bounded depression.

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

## ARR-30 — Chocolate distribution

Practice: [Open problem](https://www.geeksforgeeks.org/problems/chocolate-distribution-problem3825/1)

### Problem statement

Given non-negative integers arr where each value is the chocolates in one packet, and an integer m, choose exactly m packets for m students, one packet per student. Minimize the difference between the largest and smallest chosen packet sizes.

### Input and expected result

The examples below name the function inputs and show the required result. For an in-place task, the result is the modified array or arrays.

### Rules and variant details

Assume 1 <= m <= arr.length. Packets cannot be divided or combined. Return the minimum difference, not the chosen packets.

### Example 1

~~~text
Input:
arr = [7, 3, 2, 4, 9, 12, 56]; m = 3

Expected result:
2
~~~

Explanation: Choosing packets with 2, 3, and 4 chocolates gives difference 2.

### Example 2

~~~text
Input:
arr = [5, 5, 5, 9]; m = 3

Expected result:
0
~~~

Explanation: Three equal-sized packets can be chosen.

### Example 3

~~~text
Input:
arr = [8, 2, 10]; m = 1

Expected result:
0
~~~

Explanation: A single chosen packet has no size difference.

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

## Day 6 review

| ID | Understood | Implemented | Validated | Complexity explained | Revisit |
| --- | --- | --- | --- | --- | --- |
| ARR-26 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-27 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-28 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-29 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-30 | [ ] | [ ] | [ ] | [ ] | [ ] |
