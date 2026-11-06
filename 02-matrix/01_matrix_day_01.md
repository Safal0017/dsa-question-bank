# Matrix — Day 1

Love Babbar DSA Cracker Sheet  
Coverage: MAT-01 to MAT-05  
Questions: 5  
Examples: 3 per question  
Solutions and algorithm hints: intentionally omitted

## Today's questions

| ID | Problem | Practice |
| --- | --- | --- |
| MAT-01 | Spiral traversal of a matrix | [Open problem](https://leetcode.com/problems/spiral-matrix/) |
| MAT-02 | Search an element in a matrix | [Open problem](https://leetcode.com/problems/search-a-2d-matrix/) |
| MAT-03 | Median in a row-wise sorted matrix | [Open problem](https://www.geeksforgeeks.org/problems/median-in-a-row-wise-sorted-matrix1527/1) |
| MAT-04 | Row with the maximum number of 1s | [Open problem](https://www.geeksforgeeks.org/problems/row-with-max-1s0023/1) |
| MAT-05 | Print matrix elements in sorted order | [Open problem](https://www.geeksforgeeks.org/problems/sorted-matrix2333/0) |

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

## MAT-01 — Spiral traversal of a matrix

Practice: [Open problem](https://leetcode.com/problems/spiral-matrix/)

### Problem statement

Given a non-empty rectangular integer matrix mat with r rows and c columns, return its elements in clockwise spiral order, beginning at the top-left cell and initially moving right.

### Input and expected result

The named inputs and required result appear in the examples below. For the rotation task, the expected result is the modified input matrix.

### Rules and variant details

Return a flat list of exactly r*c values. Visit each cell exactly once. The matrix need not be square. Do not modify the input.

### Example 1

~~~text
Input:
mat = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]

Expected result:
[1, 2, 3, 6, 9, 8, 7, 4, 5]
~~~

Explanation: Read the outside boundary clockwise, then the center.

### Example 2

~~~text
Input:
mat = [[1, 2, 3, 4], [5, 6, 7, 8]]

Expected result:
[1, 2, 3, 4, 8, 7, 6, 5]
~~~

Explanation: All eight cells are visited once.

### Example 3

~~~text
Input:
mat = [[3], [2], [1]]

Expected result:
[3, 2, 1]
~~~

Explanation: A single-column matrix is read top to bottom.

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

## MAT-02 — Search an element in a matrix

Practice: [Open problem](https://leetcode.com/problems/search-a-2d-matrix/)

### Problem statement

Given a non-empty rectangular integer matrix mat and an integer target, return true if target occurs in mat; otherwise return false. Each row is sorted in non-decreasing order, and the first value of each row after the first is greater than the last value of the previous row.

### Input and expected result

The named inputs and required result appear in the examples below. For the rotation task, the expected result is the modified input matrix.

### Rules and variant details

This pack uses the globally row-major-sorted Search a 2D Matrix variant. It is not the weaker condition that only individual rows and columns are sorted. Return a boolean, not coordinates. The linked judge requests O(log(r*c)) time.

### Example 1

~~~text
Input:
mat = [[1, 3, 5, 7], [10, 11, 16, 20], [23, 30, 34, 60]]; target = 3

Expected result:
true
~~~

Explanation: 3 occurs in the first row.

### Example 2

~~~text
Input:
mat = [[1, 3, 5, 7], [10, 11, 16, 20], [23, 30, 34, 60]]; target = 13

Expected result:
false
~~~

Explanation: 13 does not occur in any cell.

### Example 3

~~~text
Input:
mat = [[8]]; target = 8

Expected result:
true
~~~

Explanation: The only cell matches.

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

## MAT-03 — Median in a row-wise sorted matrix

Practice: [Open problem](https://www.geeksforgeeks.org/problems/median-in-a-row-wise-sorted-matrix1527/1)

### Problem statement

Given a non-empty rectangular integer matrix mat whose rows are individually sorted in non-decreasing order, return the median of all its values. Both the number of rows and the number of columns are odd.

### Input and expected result

The named inputs and required result appear in the examples below. For the rotation task, the expected result is the modified input matrix.

### Rules and variant details

Columns need not be sorted. Row boundaries need not be globally ordered. Count duplicate occurrences separately. The odd total number of elements gives a single middle value, not an average. Do not change the matrix for this practice exercise.

### Example 1

~~~text
Input:
mat = [[1, 3, 5], [2, 6, 9], [3, 6, 9]]

Expected result:
5
~~~

Explanation: The combined sorted values are [1, 2, 3, 3, 5, 6, 6, 9, 9]; the fifth value is 5.

### Example 2

~~~text
Input:
mat = [[1, 1, 1], [2, 2, 2], [2, 3, 4]]

Expected result:
2
~~~

Explanation: The fifth value is 2; repeated values occupy separate positions.

### Example 3

~~~text
Input:
mat = [[3], [8], [4]]

Expected result:
4
~~~

Explanation: The ordered values are [3, 4, 8]. The column itself need not be sorted.

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

## MAT-04 — Row with the maximum number of 1s

Practice: [Open problem](https://www.geeksforgeeks.org/problems/row-with-max-1s0023/1)

### Problem statement

Given a non-empty rectangular binary matrix mat with each row sorted in non-decreasing order, return the zero-based index of the row containing the greatest number of 1s.

### Input and expected result

The named inputs and required result appear in the examples below. For the rotation task, the expected result is the modified input matrix.

### Rules and variant details

If multiple rows tie, return the smallest row index. If every row contains only zeros, return -1. Return the row index, not the number of ones. Columns are not required to be sorted.

### Example 1

~~~text
Input:
mat = [[0, 1, 1, 1], [0, 0, 1, 1], [1, 1, 1, 1]]

Expected result:
2
~~~

Explanation: Row 2 has four ones, more than any other row.

### Example 2

~~~text
Input:
mat = [[0, 1, 1], [0, 1, 1], [0, 0, 1]]

Expected result:
0
~~~

Explanation: Rows 0 and 1 tie with two ones; choose index 0.

### Example 3

~~~text
Input:
mat = [[0, 0], [0, 0]]

Expected result:
-1
~~~

Explanation: There are no ones anywhere.

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

## MAT-05 — Print matrix elements in sorted order

Practice: [Open problem](https://www.geeksforgeeks.org/problems/sorted-matrix2333/0)

### Problem statement

Given a non-empty n by n integer matrix mat in which every row and every column is sorted in non-decreasing order, return all n*n elements as one non-decreasing list.

### Input and expected result

The named inputs and required result appear in the examples below. For the rotation task, the expected result is the modified input matrix.

### Rules and variant details

Preserve repeated occurrences. Row-and-column ordering does not mean that reading the original rows consecutively is already globally sorted. This pack returns a flat list to match the sheet title. If the linked judge asks for a sorted matrix, fill that matrix row by row using the same ordered sequence.

### Example 1

~~~text
Input:
mat = [[10, 20, 30], [15, 25, 35], [24, 29, 37]]

Expected result:
[10, 15, 20, 24, 25, 29, 30, 35, 37]
~~~

Explanation: The returned list contains every cell in global sorted order.

### Example 2

~~~text
Input:
mat = [[1, 2], [2, 3]]

Expected result:
[1, 2, 2, 3]
~~~

Explanation: Both occurrences of 2 remain.

### Example 3

~~~text
Input:
mat = [[7]]

Expected result:
[7]
~~~

Explanation: A one-cell matrix contributes one value.

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

## Day 1 review

| ID | Understood | Implemented | Validated | Complexity explained | Revisit |
| --- | --- | --- | --- | --- | --- |
| MAT-01 | [ ] | [ ] | [ ] | [ ] | [ ] |
| MAT-02 | [ ] | [ ] | [ ] | [ ] | [ ] |
| MAT-03 | [ ] | [ ] | [ ] | [ ] | [ ] |
| MAT-04 | [ ] | [ ] | [ ] | [ ] | [ ] |
| MAT-05 | [ ] | [ ] | [ ] | [ ] | [ ] |
