========== Question ==========  

### Lowest Common Ancestor of a Binary Search Tree

Given a binary search tree (BST), find the lowest common ancestor (LCA) node of two given nodes in the BST.

According to the [definition of LCA on Wikipedia](https://en.wikipedia.org/wiki/Lowest_common_ancestor): “The lowest common ancestor is defined between two nodes `p` and `q` as the lowest node in `T` that has both `p` and `q` as descendants (where we allow **a node to be a descendant of itself**).”

**Example 1:**

![image](https://imagedelivery.net/CLfkmk9Wzy8_9HRyug4EVA/6a944957-3b32-4eab-37ab-48b701a70000/public)

```
Input: root = [6,2,8,0,4,7,9,null,null,3,5], p = 2, q = 8
Output: 6
Explanation: The LCA of nodes 2 and 8 is 6.
```

**Example 2:**

![image](https://imagedelivery.net/CLfkmk9Wzy8_9HRyug4EVA/fe9f02bd-c21c-4dac-d6c5-1962775c0800/public)

```
Input: root = [6,2,8,0,4,7,9,null,null,3,5], p = 2, q = 4
Output: 2
Explanation: The LCA of nodes 2 and 4 is 2, since a node can be a descendant of itself according to the LCA definition.
```

**Example 3:**

```
Input: root = [2,1], p = 2, q = 1
Output: 2
```

**Constraints:**

-   The number of nodes in the tree is in the range `[2, 10^5]`.

-   `10^9 <= Node.val <= 10^9`

-   All `Node.val` are **unique**.

-   `p != q`

-   `p` and `q` will exist in the BST.

---

Given the below Python function to solve the problem, what are the time and space complexities? Assume there are `n` nodes in the tree and the tree is balanced.

```python
class Solution:
    def lowestCommonAncestor(self, root: 'TreeNode', p: 'TreeNode', q: 'TreeNode') -> 'TreeNode':
        cur = root

        while cur:
            if p.val > cur.val and q.val > cur.val:
                cur = cur.right
            elif p.val < cur.val and q.val < cur.val:
                cur = cur.left
            else:
                return cur
```

A) Time complexity: O(log n), Space complexity: O(log n)

B) Time complexity: O(log n), Space complexity: O(1)

C) Time complexity: O(n), Space complexity: O(1)  

========== Answer ==========  

**Answer**: B

The time complexity of this solution is O(log n), where n is the number of nodes in the tree. This is because we are essentially performing a binary search, narrowing down our search to either the left or right subtrees each time, which gives a log(n) time complexity. The space complexity is O(1), because this approach only uses a constant amount of space and doesn't depend on the size of the input tree.

========== Id ==========  
177

---

DECK INFO

TARGET DECK: Data Structures and Algorithms::Leetcode::MNAB - Neetcode 150 and blind 75 - multi-author::Part VII - Trees::Chapter 7 - Lowest Common Ancestor of a Binary Search Tree - Blind

FILE TAGS: #DSA::#Leetcode::#MNAB-Neetcode-150-and-blind-75-multi-author::#Part-VII-Trees::#Chapter-7-Lowest-Common-Ancestor-of-a-Binary-Search-Tree-Blind::#177-Lowest-common-ancestor-of-a-binary-search

Tags:

Reference:

Related:

```dataview
LIST
where file.name = this.file.name
```

QUESTION STATUS: Safe to store
