========== Question ==========  

### Rotate Image

You are given an `n x n` 2D `matrix` representing an image, rotate the image by **90** degrees (clockwise).

You have to rotate the image **[in-place](https://en.wikipedia.org/wiki/In-place_algorithm)**, which means you have to modify the input 2D matrix directly. **DO NOT** allocate another 2D matrix and do the rotation.

**Example 1:**

![image](https://imagedelivery.net/CLfkmk9Wzy8_9HRyug4EVA/0e39a867-7e9c-4189-2b4e-1f6335868600/public)

```
Input: matrix = [[1,2,3],[4,5,6],[7,8,9]]
Output: [[7,4,1],[8,5,2],[9,6,3]]
```

**Example 2:**

![image](https://imagedelivery.net/CLfkmk9Wzy8_9HRyug4EVA/a7e0dfba-646e-423e-2c4e-a6f0dfc2a500/public)

```
Input: matrix = [[5,1,9,11],[2,4,8,10],[13,3,6,7],[15,14,12,16]]
Output: [[15,13,2,5],[14,3,4,1],[12,6,8,9],[16,7,10,11]]
```

**Constraints:**

-   `n == matrix.length == matrix[i].length`

-   `1 <= n <= 20`

-   `1000 <= matrix[i][j] <= 1000`

---

Given an `n x n` square matrix, how many layers will we have to rotate?

A) n layers

B) n/2 layers

C) 2n layers

D) n^2 layers  

========== Answer ==========  

**Answer**: B

For an nxn matrix, we only need to rotate n/2 layers. This is because with each layer, we are actually rotating 4 sides (top, right, bottom, left) of the square matrix.

========== Id ==========  
236

---

DECK INFO

TARGET DECK: Data Structures and Algorithms::Leetcode::MNAB - Neetcode 150 and blind 75 - multi-author::Part XVIII - Math Geometry::Chapter 1 - Rotate Image - Blind

FILE TAGS: #DSA::#Leetcode::#MNAB-Neetcode-150-and-blind-75-multi-author::#Part-XVIII-Math-Geometry::#Chapter-1-Rotate-Image-Blind::#236-Rotate-image-you-are-given-an-n-x-n-2d

Tags:

Reference:

Related:

```dataview
LIST
where file.name = this.file.name
```

QUESTION STATUS: Safe to store
