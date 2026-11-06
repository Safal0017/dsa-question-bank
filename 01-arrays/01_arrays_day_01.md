# Arrays — Day 1

Love Babbar DSA Cracker Sheet  
Coverage: ARR-01 to ARR-05  
Questions: 5  
Examples: 3 per question  
Solutions and algorithm hints: intentionally omitted

## Today's questions

| ID | Problem | Practice |
| --- | --- | --- |
| ARR-01 | Reverse the array | [GFG](https://www.geeksforgeeks.org/problems/reverse-an-array/1) |
| ARR-02 | Find the minimum and maximum element | [GFG](https://www.geeksforgeeks.org/problems/find-minimum-and-maximum-element-in-an-array4428/1) |
| ARR-03 | Find the kth smallest and kth largest element | [GFG: kth smallest](https://www.geeksforgeeks.org/problems/kth-smallest-element5635/1) |
| ARR-04 | Sort an array containing only 0s, 1s and 2s | [GFG](https://www.geeksforgeeks.org/problems/sort-an-array-of-0s-1s-and-2s4231/1) |
| ARR-05 | Move negative elements to the end, preserving order | [GFG](https://www.geeksforgeeks.org/problems/move-all-negative-elements-to-end1813/1) |

## How to use this pack

For each question:

1. Read the statement and clarify exactly what the output represents.
2. Dry-run the three examples manually.
3. Derive a straightforward correct approach.
4. Implement it and validate the examples.
5. Look for improvements in time or auxiliary space.
6. Test additional edge cases.
7. Record the final time and auxiliary-space complexity.

Do not open editorials or article solutions before attempting the problem.

Conventions:
- `n` means `arr.length`.
- Array displays below describe function inputs and expected results, not a platform's stdin format.
- Numeric constraints follow the linked GFG versions checked during preparation.
- Examples are selected for this practice pack; they are not all copied from the platform.
- Any additional rule or difference from the linked judge is explicitly stated.

---

## ARR-01 — Reverse the array

### Problem statement

Given an integer array `arr`, reverse the order of all its elements.

Modify the supplied array itself. Merely printing its elements backwards does not satisfy the requirement.

### Input and expected result

Input:
- An integer array `arr` of length `n`.

Expected result:
- The same array after reversal.
- If your function uses a void return type, update `arr` directly; no separate returned array is necessary.

### Rules

- The last element becomes the first.
- The second-last element becomes the second, and so on.
- Every original value must remain, with the same frequency.
- An array containing one element remains unchanged.

### Constraints

- `1 <= n <= 100000`
- `0 <= arr[i] <= 100000`

### Example 1 — Even-length array

~~~text
Input:
arr = [1, 4, 3, 2, 6, 5]

Expected array:
[5, 6, 2, 3, 4, 1]
~~~

Explanation: The entire sequence is reversed, including the two middle positions.

### Example 2 — Odd length with duplicates

~~~text
Input:
arr = [8, 0, 8, 2, 2]

Expected array:
[2, 2, 8, 0, 8]
~~~

Explanation: Duplicate values remain duplicated. The middle element stays in the middle.

### Example 3 — One element

~~~text
Input:
arr = [7]

Expected array:
[7]
~~~

Explanation: There is only one position, so nothing changes.

### Requirement check

This is whole-array reversal, not rotation and not reversal in groups.

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

## ARR-02 — Find the minimum and maximum element

### Problem statement

Given a non-empty integer array `arr`, find its smallest value and largest value.

Return them in the order:

~~~text
[minimum, maximum]
~~~

### Input and expected result

Input:
- An integer array `arr` of length `n`.

Output:
- A pair containing the minimum and maximum values.

Return the values, not their indices. You do not need to rearrange the array.

### Rules

- Duplicate values are allowed.
- If every element is equal, the minimum and maximum are equal.
- For a one-element array, that element is both the minimum and maximum.

### Constraints

- `1 <= n <= 100000`
- `1 <= arr[i] <= 1000000000`

### Example 1 — Unsorted values

~~~text
Input:
arr = [12, 3, 15, 7, 9]

Output:
[3, 15]
~~~

Explanation: The smallest value is `3`; the largest is `15`.

### Example 2 — All values equal

~~~text
Input:
arr = [6, 6, 6, 6]

Output:
[6, 6]
~~~

Explanation: Both extrema are `6`, regardless of how many times it occurs.

### Example 3 — One element

~~~text
Input:
arr = [42]

Output:
[42, 42]
~~~

Explanation: The sole value is both the minimum and maximum.

### Requirement check

Return the two extrema—not their sum, difference or positions.

The separate Searching and Sorting entry about minimising comparisons remains a separate exercise in the index.

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

## ARR-03 — Find the kth smallest and kth largest element

### Problem statement

Given an integer array `arr` and an integer `k`, find:

1. The kth smallest value.
2. The kth largest value.

Ranks are 1-based. Repeated occurrences count separately.

For this practice pack, return:

~~~text
[kthSmallest, kthLargest]
~~~

### Platform difference

The sheet title asks for both kth smallest and kth largest.

The linked GFG judge asks only for kth smallest:
- For this pack, solve both parts.
- For submission to that GFG page, return only `kthSmallest`.

The pair above is this pack's documented output format, not the GFG function signature.

### Input and expected result

Input:
- An integer array `arr` of length `n`.
- A valid integer rank `k`.

Output:
- `[kthSmallest, kthLargest]`.

### Rules

- Count occurrences, not distinct values.
- For `[2, 2, 5]`, the second-smallest value is `2`.
- The kth largest is counted from the largest end.
- The input is not guaranteed to be sorted.
- This exercise does not prohibit modifying the input array.

### Constraints

- `1 <= n <= 100000`
- `1 <= arr[i] <= 100000`
- `1 <= k <= n`

### Example 1 — Different answers for the two ranks

~~~text
Input:
arr = [7, 10, 4, 3, 20, 15]
k = 3

Output:
[7, 10]
~~~

Explanation:

The values in ascending order are:

~~~text
[3, 4, 7, 10, 15, 20]
~~~

The third-smallest value is `7`.  
The third-largest value is `10`.

The ordered display explains the expected result; it does not prescribe your implementation.

### Example 2 — Duplicates occupy separate ranks

~~~text
Input:
arr = [5, 2, 2, 9, 9]
k = 2

Output:
[2, 9]
~~~

Explanation:

In ascending order:

~~~text
[2, 2, 5, 9, 9]
~~~

The second-smallest value is `2`, not `5`.  
The second-largest value is `9`, not `5`.

### Example 3 — One element

~~~text
Input:
arr = [8]
k = 1

Output:
[8, 8]
~~~

Explanation: The first-smallest and first-largest values are both `8`.

### Requirement check

Do not assume all elements are distinct. The current linked GFG statement permits repeated values.

### My working area

- Straightforward approach:
- Improved approach:
- Time complexity:
- Auxiliary-space complexity:
- Additional tests:
- Mistakes or observations:

- [ ] Implemented both parts
- [ ] All three examples passed
- [ ] Tested `k = 1` and `k = n`
- [ ] Can explain correctness and complexity

---

## ARR-04 — Sort an array containing only 0s, 1s and 2s

### Problem statement

Given an array `arr` containing only `0`, `1` and `2`, rearrange it into non-decreasing order.

Modify the original array.

Do not use a built-in sort function or a general-purpose comparison-sorting algorithm.

### Input and expected result

Input:
- An array `arr` of length `n`.
- Every element is `0`, `1` or `2`.

Expected result:
- All `0`s first.
- Then all `1`s.
- Then all `2`s.

### Rules

- Preserve the number of occurrences of each value.
- One or two of the possible values may be absent.
- Do not introduce missing values into the output.

### Constraints

- `1 <= n <= 100000`
- `0 <= arr[i] <= 2`

### Example 1 — All three values present

~~~text
Input:
arr = [2, 0, 2, 1, 1, 0]

Expected array:
[0, 0, 1, 1, 2, 2]
~~~

Explanation: The input contains two occurrences of each value.

### Example 2 — No 1s present

~~~text
Input:
arr = [2, 2, 0, 2, 0]

Expected array:
[0, 0, 2, 2, 2]
~~~

Explanation: The output contains two `0`s and three `2`s. No `1` should be added.

### Example 3 — One element

~~~text
Input:
arr = [1]

Expected array:
[1]
~~~

Explanation: A one-element array is already ordered.

### Requirement check

The sheet's phrase “without using any sorting algo” means not applying a general-purpose sorting routine. The required final array is still sorted.

Optional follow-up from the linked GFG problem:

Can you solve it in one pass using constant auxiliary space?

Attempt the basic requirement before working on the follow-up.

### My working area

- Straightforward approach:
- Improved approach:
- Time complexity:
- Auxiliary-space complexity:
- Additional tests:
- Mistakes or observations:

- [ ] Implemented without a general-purpose sort
- [ ] All three examples passed
- [ ] Additional edge cases passed
- [ ] Can explain correctness and complexity

---

## ARR-05 — Move negative elements to the end, preserving order

### Problem statement

Given an integer array `arr`, move every negative value to the end.

Preserve:
1. The original relative order of the non-negative values.
2. The original relative order of the negative values.

Write the result back into the supplied array.

### Variant used in this pack

The sheet broadly says:

> Move all negative elements to one side of the array.

Its linked GFG problem is more specific:

> Move negatives to the end while preserving relative order.

This pack follows that linked variant.

An answer with negatives at the beginning, or with either group's internal order changed, does not satisfy this pack.

### Input and expected result

Input:
- An integer array `arr` of length `n`.

Expected result:
- All values `>= 0`, in their original relative order.
- Followed by all values `< 0`, in their original relative order.

The GFG function updates the array rather than returning a separate result.

### Rules

- Zero belongs to the non-negative group.
- Preserve every original occurrence.
- Do not sort either group.
- An array with no negative values remains unchanged.
- An array containing only negative values remains unchanged.

Space requirement for this pack:
- Update the supplied array.
- No O(1) auxiliary-space target is imposed here.
- A void return type alone does not mean temporary storage is forbidden.

### Constraints

- `1 <= n <= 1000000`
- `-1000000000 <= arr[i] <= 1000000000`

### Example 1 — Mixed signs

~~~text
Input:
arr = [1, -1, 3, 2, -7, -5, 11, 6]

Expected array:
[1, 3, 2, 11, 6, -1, -7, -5]
~~~

Explanation:

The non-negative values retain this order:

~~~text
1, 3, 2, 11, 6
~~~

The negative values retain this order:

~~~text
-1, -7, -5
~~~

### Example 2 — Zero and negative values

~~~text
Input:
arr = [-4, 0, 5, -2, 0]

Expected array:
[0, 5, 0, -4, -2]
~~~

Explanation: Both zeros belong to the non-negative group. Neither group's original relative order changes.

### Example 3 — All values negative

~~~text
Input:
arr = [-8, -3, -8]

Expected array:
[-8, -3, -8]
~~~

Explanation: Every value is already in the negative group. Preserving their order means leaving the array unchanged.

### Requirement check

For Example 1, this is not valid:

~~~text
[6, 11, 2, 3, 1, -1, -7, -5]
~~~

Although negatives are at the end, the non-negative group's relative order has changed.

### My working area

- Straightforward approach:
- Improved approach:
- Time complexity:
- Auxiliary-space complexity:
- Additional tests:
- Mistakes or observations:

- [ ] Implemented the stable negatives-at-end variant
- [ ] All three examples passed
- [ ] Tested an array with no negatives
- [ ] Can explain correctness and complexity

---

## Day 1 review

| ID | Understood | Implemented | Validated | Complexity explained | Revisit |
| --- | --- | --- | --- | --- | --- |
| ARR-01 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-02 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-03 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-04 | [ ] | [ ] | [ ] | [ ] | [ ] |
| ARR-05 | [ ] | [ ] | [ ] | [ ] | [ ] |

## Remaining Arrays packs

These are planned, not included in this delivery.

| Pack | Questions | Count |
| --- | --- | ---: |
| Day 2 | ARR-06–ARR-10 | 5 |
| Day 3 | ARR-11–ARR-15 | 5 |
| Day 4 | ARR-16–ARR-20 | 5 |
| Day 5 | ARR-21–ARR-25 | 5 |
| Day 6 | ARR-26–ARR-30 | 5 |
| Day 7 | ARR-31–ARR-36 | 6 |

Total Arrays coverage after all seven packs: 36 sheet entries.