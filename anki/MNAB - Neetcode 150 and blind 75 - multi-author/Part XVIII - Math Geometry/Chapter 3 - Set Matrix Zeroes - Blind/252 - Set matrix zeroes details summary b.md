========== Question ==========  

### Set Matrix Zeroes

<details><summary><b>📄 Description</b></summary><br>

Given an `m x n` matrix of integers `matrix`, if an element is `0`, set its entire row and column to `0`'s.

You must update the matrix _in-place_.

**Follow up:** Could you solve it using `O(1)` space?

**Example 1:**

![](https://imagedelivery.net/CLfkmk9Wzy8_9HRyug4EVA/49ffd14e-b32b-4ed8-e0d0-9378e5eb9b00/public)

```
Input: matrix = [
  [0,1],
  [1,0]
]

Output: [
  [0,0],
  [0,0]
]
```

**Example 2:**

![](https://imagedelivery.net/CLfkmk9Wzy8_9HRyug4EVA/04d99cc8-e453-464d-888c-58d0a95daf00/public)

```
Input: matrix = [
  [1,2,3],
  [4,0,5],
  [6,7,8]
]

Output: [
  [1,0,3],
  [0,0,0],
  [6,0,8]
]
```

**Constraints:**

-   `1 <= matrix.length, matrix[0].length <= 100`

-   `-2^31 <= matrix[i][j] <= (2^31) - 1`

</details>

---

What would happen if we don't separately track whether the first row/column originally contained zeros?

A) The algorithm would still work correctly

B) Some rows or columns might not be properly zeroed

C) The entire matrix would be zeroed incorrectly

D) The algorithm would enter an infinite loop  

========== Answer ==========  

**Answer**: C

If we don't separately track whether the first row/column originally contained zeros, we would incorrectly zero out rows and columns based on our markers. Since we're using the first row and column as markers, they might be set to zero during the marking phase even if they didn't originally contain zeros, leading to incorrect zeroing of the entire matrix.

========== Id ==========  
252

---

DECK INFO

TARGET DECK: Data Structures and Algorithms::Leetcode::MNAB - Neetcode 150 and blind 75 - multi-author::Part XVIII - Math Geometry::Chapter 3 - Set Matrix Zeroes - Blind

FILE TAGS: #DSA::#Leetcode::#MNAB-Neetcode-150-and-blind-75-multi-author::#Part-XVIII-Math-Geometry::#Chapter-3-Set-Matrix-Zeroes-Blind::#252-Set-matrix-zeroes-details-summary-b

Tags:

Reference:

Related:

```dataview
LIST
where file.name = this.file.name
```

QUESTION STATUS: Safe to store
