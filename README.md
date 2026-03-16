# 🌳 Lowest Common Ancestor in a Binary Tree

## 📌 Overview

This project implements the **Lowest Common Ancestor (LCA)** problem for a **Binary Tree**.

The **Lowest Common Ancestor** of two nodes is defined as the **lowest node in the tree that has both nodes as descendants** (where a node can also be a descendant of itself).

This problem is widely used in **tree-based algorithms and technical interviews**.

---

# 🎯 Problem Statement

Given:

* The **root** of a binary tree
* Two nodes `n1` and `n2`

Find the **lowest common ancestor** of these two nodes.

---

# 🌿 Example

Binary Tree:

```id="tree_lca"
        1
       / \
      2   3
     / \ / \
    4  5 6  7
```

If:

```id="example_nodes"
n1 = 4
n2 = 7
```

The paths from root to nodes are:

```id="paths"
Path to 4 → 1 → 2 → 4
Path to 7 → 1 → 3 → 7
```

The **last common node** in both paths is:

```id="lca_result"
1
```

So the **Lowest Common Ancestor = 1**

---

# ⚙️ Approach

The solution follows a **Path Comparison Method**.

### Step 1 — Find Path to First Node

Traverse the tree and store the path from the **root to node `n1`**.

---

### Step 2 — Find Path to Second Node

Similarly, find the path from the **root to node `n2`**.

---

### Step 3 — Compare Both Paths

Compare both stored paths node by node.

* Continue while nodes are the same.
* The **last matching node** is the **Lowest Common Ancestor**.

---

# 🔁 Algorithm Workflow

```id="workflow_lca"
Binary Tree
     ↓
Find path from root → n1
     ↓
Find path from root → n2
     ↓
Compare both paths
     ↓
Last common node = LCA
```

---

# ⏱ Time and Space Complexity

| Complexity       | Value |
| ---------------- | ----- |
| Time Complexity  | O(n)  |
| Space Complexity | O(n)  |

Where:

* **n** = number of nodes in the binary tree

Explanation:

* Traversing the tree to find both paths takes **O(n)** time.
* Storing paths requires **O(n)** space in the worst case.

---

# 🧠 Concepts Used

* 🌳 Binary Trees
* 🔁 Recursion
* 📂 Path Tracking
* 🔍 Tree Traversal
* 📊 ArrayList for storing paths

---

# 🎯 Learning Outcomes

After completing this problem you will understand:

✔ How to find paths in a binary tree
✔ How to compare paths to determine a common ancestor
✔ Recursive tree traversal techniques
✔ Practical implementation of tree algorithms

These concepts are essential for **Data Structures and Algorithms (DSA)** and **technical interview preparation**.

---

# 👨‍💻 Author

Developed as part of **Data Structures and Algorithms practice** 🚀
