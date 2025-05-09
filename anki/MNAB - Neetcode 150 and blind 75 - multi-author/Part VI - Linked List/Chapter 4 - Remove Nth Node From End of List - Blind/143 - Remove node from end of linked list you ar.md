========== Question ==========  

### Remove Node From End of Linked List

You are given the beginning of a linked list `head`, and an integer `n`.

Remove the `nth` node from the end of the list and return the beginning of the list.

**Example 1:**

```
Input: head = [1,2,3,4], n = 2

Output: [1,2,4]
```

**Example 2:**

```
Input: head = [5], n = 1

Output: []
```

**Example 3:**

```
Input: head = [1,2], n = 2

Output: [2]
```

**Constraints:**

-   The number of nodes in the list is `sz`.

-   `1 <= sz <= 30`

-   `0 <= Node.val <= 100`

-   `1 <= n <= sz`

---

An edge case is where we must remove the first node in the list. What is a simple way to eliminate this edge case?

A) Add a dummy node at the end of the list.

B) Add a dummy node at the beginning of the list.

C) There is no way to eliminate this edge case.  

========== Answer ==========  

**Answer**: B

To eliminate the edge case of removing the first node in the list, we can add a dummy node at the beginning of the list. This dummy node won't affect the other operations, but allows us to handle the head of the list in a consistent way with other nodes.

========== Id ==========  
143

---

DECK INFO

TARGET DECK: Data Structures and Algorithms::Leetcode::MNAB - Neetcode 150 and blind 75 - multi-author::Part VI - Linked List::Chapter 4 - Remove Nth Node From End of List - Blind

FILE TAGS: #DSA::#Leetcode::#MNAB-Neetcode-150-and-blind-75-multi-author::#Part-VI-Linked-List::#Chapter-4-Remove-Nth-Node-From-End-of-List-Blind::#143-Remove-node-from-end-of-linked-list-you-ar

Tags:

Reference:

Related:

```dataview
LIST
where file.name = this.file.name
```

QUESTION STATUS: Safe to store
