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

After we have created the offset, by how much should we shift each pointer on each iteration of the loop?

A) First pointer by 1, Second pointer by 2

B) First pointer by 1, Second pointer by 1  

========== Answer ==========  

**Answer**: B

After we have created the offset, we should shift each pointer by 1 on each iteration of the loop. This ensures that the offset (the gap between the two pointers) remains constant while traversing the list, allowing us to find the node to be removed.

========== Id ==========  
145

---

DECK INFO

TARGET DECK: Data Structures and Algorithms::Leetcode::MNAB - Neetcode 150 and blind 75 - multi-author::Part VI - Linked List::Chapter 4 - Remove Nth Node From End of List - Blind

FILE TAGS: #DSA::#Leetcode::#MNAB-Neetcode-150-and-blind-75-multi-author::#Part-VI-Linked-List::#Chapter-4-Remove-Nth-Node-From-End-of-List-Blind::#145-Remove-node-from-end-of-linked-list-you-ar

Tags:

Reference:

Related:

```dataview
LIST
where file.name = this.file.name
```

QUESTION STATUS: Safe to store
