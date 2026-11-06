# Matrix — Day 2

Love Babbar DSA Cracker Sheet  
Coverage: MAT-06 to MAT-10  
Questions: 5  
Examples: 3 per question  
Solutions and algorithm hints: intentionally omitted

## Today's questions

| ID | Problem | Practice |
| --- | --- | --- |
| MAT-06 | Maximum-area rectangle containing only 1s | [Open problem](https://www.geeksforgeeks.org/problems/max-rectangle/1) |
| MAT-07 | Find a specific pair in a matrix | [Open problem](https://www.geeksforgeeks.org/problems/maximum-difference-between-pair-in-a-matrix/1) |
| MAT-08 | Rotate a matrix by 90 degrees | [Open problem](https://leetcode.com/problems/rotate-image/) |
| MAT-09 | Kth smallest element in a sorted matrix | [Open problem](https://www.geeksforgeeks.org/problems/kth-element-in-matrix/1) |
| MAT-10 | Common elements in all rows | [Open problem](https://www.geeksforgeeks.org/dsa/common-elements-in-all-rows-of-a-given-matrix/) |

## Conventions

- `r` and `c` denote row and column counts; `n` denotes the side length of a square matrix.
- All indices are zero-based unless a rank is explicitly described as one-based.
- Every matrix is non-empty and rectangular; ragged rows are outside these exercises.
- Displays describe function inputs and expected results, not platform stdin format.
- Examples are prepared for this pack, not necessarily copied from a platform.
- Rules below define the selected practice variant; platform differences are stated explicitly.
- Current numeric judge limits are available on the linked pages; no claim is made here to reproduce all platform constraints.
- Practice links can contain editorials or solutions. Attempt the problem before opening those sections.

---

## MAT-06 — Maximum-area rectangle containing only 1s

Practice: [Open problem](https://www.geeksforgeeks.org/problems/max-rectangle/1)

### Problem statement

Given a non-empty rectangular binary matrix mat, return the largest area of an axis-aligned rectangle consisting entirely of 1s.

### Input and expected result

The named inputs and required result appear in the examples below. For the rotation task, the expected result is the modified input matrix.

### Rules and variant details

A rectangle uses consecutive rows and consecutive columns. Area is its height multiplied by its width. It need not be a square. Return 0 if there are no ones. Do not rearrange rows or columns.

### Example 1

~~~text
Input:
mat = [[0, 1, 1, 0], [1, 1, 1, 1], [1, 1, 1, 1], [1, 1, 0, 0]]

Expected result:
8
~~~

Explanation: Rows 1 through 2 and columns 0 through 3 form a 2-by-4 rectangle.

### Example 2

~~~text
Input:
mat = [[0, 0, 0], [0, 0, 0]]

Expected result:
0
~~~

Explanation: No rectangle of ones exists.

### Example 3

~~~text
Input:
mat = [[1, 1, 0, 1]]

Expected result:
2
~~~

Explanation: The first two cells form the largest valid rectangle.

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

## MAT-07 — Find a specific pair in a matrix

Practice: [Open problem](https://www.geeksforgeeks.org/problems/maximum-difference-between-pair-in-a-matrix/1)

### Problem statement

Given an n by n integer matrix mat with n >= 2, return the maximum value of mat[c][d] - mat[a][b] over all choices satisfying c > a and d > b.

### Input and expected result

The named inputs and required result appear in the examples below. For the rotation task, the expected result is the modified input matrix.

### Rules and variant details

The second cell must be strictly below AND strictly to the right of the first cell. Neither shared rows nor shared columns qualify. Return the maximum difference, not the pair of values or coordinates. A valid pair must be selected even if every difference is negative. The matrix is not assumed sorted.

### Example 1

~~~text
Input:
mat = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]

Expected result:
8
~~~

Explanation: Choose (a,b) = (0,0) and (c,d) = (2,2): 9 - 1 = 8.

### Example 2

~~~text
Input:
mat = [[5, 9], [7, 2]]

Expected result:
-3
~~~

Explanation: The only valid pair is (0,0) followed by (1,1): 2 - 5 = -3.

### Example 3

~~~text
Input:
mat = [[10, 1, 2], [3, 4, 8], [5, 6, 7]]

Expected result:
7
~~~

Explanation: Choose (0,1) followed by (1,2): 8 - 1 = 7.

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

## MAT-08 — Rotate a matrix by 90 degrees

Practice: [Open problem](https://leetcode.com/problems/rotate-image/)

### Problem statement

Given a non-empty n by n integer matrix mat, rotate it 90 degrees clockwise and update the supplied matrix.

### Input and expected result

The named inputs and required result appear in the examples below. For the rotation task, the expected result is the modified input matrix.

### Rules and variant details

This pack explicitly uses clockwise rotation. Use O(1) auxiliary space; do not allocate a second n-by-n matrix. The matrix is square, not rectangular. Return behavior may be void; the required result is the modified matrix.

### Example 1

~~~text
Input:
mat = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]

Expected result:
[[7, 4, 1], [8, 5, 2], [9, 6, 3]]
~~~

Explanation: The original first column becomes the top row in reverse order.

### Example 2

~~~text
Input:
mat = [[1, 2], [3, 4]]

Expected result:
[[3, 1], [4, 2]]
~~~

Explanation: The original bottom-left cell moves to the top-left.

### Example 3

~~~text
Input:
mat = [[5]]

Expected result:
[[5]]
~~~

Explanation: A single cell remains unchanged.

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

## MAT-09 — Kth smallest element in a sorted matrix

Practice: [Open problem](https://www.geeksforgeeks.org/problems/kth-element-in-matrix/1)

### Problem statement

Given a non-empty n by n integer matrix mat whose rows and columns are sorted in non-decreasing order, and an integer k with 1 <= k <= n*n, return the kth smallest value among all cells.

### Input and expected result

The named inputs and required result appear in the examples below. For the rotation task, the expected result is the modified input matrix.

### Rules and variant details

Ranks are one-based. Count repeated occurrences separately; this is not the kth distinct value. Return a value, not its coordinates. The concatenated original rows are not necessarily globally sorted.

### Example 1

~~~text
Input:
mat = [[1, 5, 9], [10, 11, 13], [12, 13, 15]]; k = 8

Expected result:
13
~~~

Explanation: The combined ordering is [1, 5, 9, 10, 11, 12, 13, 13, 15].

### Example 2

~~~text
Input:
mat = [[1, 2], [2, 3]]; k = 3

Expected result:
2
~~~

Explanation: The two occurrences of 2 occupy ranks 2 and 3.

### Example 3

~~~text
Input:
mat = [[7]]; k = 1

Expected result:
7
~~~

Explanation: There is only one ranked value.

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

## MAT-10 — Common elements in all rows

Practice: [Open problem](https://www.geeksforgeeks.org/dsa/common-elements-in-all-rows-of-a-given-matrix/)

### Problem statement

Given a non-empty rectangular integer matrix mat, return the distinct values that occur in every row. Return them in increasing order for a deterministic result.

### Input and expected result

The named inputs and required result appear in the examples below. For the rotation task, the expected result is the modified input matrix.

### Rules and variant details

Rows and columns are not assumed sorted. A repeated value in one row does not replace its absence from another row. Return each qualifying value once. Return an empty list if no value appears in all rows. The linked GFG article describes printing the values in any order; this pack returns them sorted. The article includes solutions, so use it only after attempting the problem.

### Example 1

~~~text
Input:
mat = [[1, 2, 1, 4], [4, 1, 3, 1], [1, 4, 4, 5]]

Expected result:
[1, 4]
~~~

Explanation: Both 1 and 4 appear in every row.

### Example 2

~~~text
Input:
mat = [[2, 2, 2], [2, 3, 3], [3, 3, 3]]

Expected result:
[]
~~~

Explanation: 2 is absent from the last row and 3 is absent from the first.

### Example 3

~~~text
Input:
mat = [[3, 1, 3, 2]]

Expected result:
[1, 2, 3]
~~~

Explanation: With one row, every distinct value in that row qualifies.

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
| MAT-06 | [ ] | [ ] | [ ] | [ ] | [ ] |
| MAT-07 | [ ] | [ ] | [ ] | [ ] | [ ] |
| MAT-08 | [ ] | [ ] | [ ] | [ ] | [ ] |
| MAT-09 | [ ] | [ ] | [ ] | [ ] | [ ] |
| MAT-10 | [ ] | [ ] | [ ] | [ ] | [ ] |
