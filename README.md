# Red-Black Tree Implementation in C

## Project Summary
This project implements a Red-Black Tree, a self-balancing Binary Search Tree (BST), using C programming.

It maintains balanced tree properties during insertion and deletion operations, ensuring efficient searching, insertion, and deletion even when the number of elements increases.

## Overview
A Red-Black Tree is a self-balancing binary search tree in which every node is assigned a color: **Red or Black**.

The tree uses specific coloring rules and rotation operations to maintain balance and control its height.

Unlike an ordinary Binary Search Tree, a Red-Black Tree prevents the tree from becoming highly unbalanced.

## Properties of Red-Black Tree

A Red-Black Tree follows five important properties:

1. Every node is either Red or Black.
2. The root node is always Black.
3. All leaf NIL nodes are Black.
4. A Red node cannot have a Red parent or Red child.
5. Every path from a node to its descendant NIL leaves contains the same number of Black nodes.

These properties help maintain a balanced tree.

## Operations Implemented

| Operation | Description |
|---|---|
| Insertion | Adds a new node while maintaining Red-Black properties |
| Deletion | Removes a node and restores tree balance |
| Searching | Searches for a particular value |
| Traversal | Visits and displays tree elements |
| Rotations | Performs left and right rotations to maintain balance |

*Keep only the operations supported by your actual implementation.*

## Working Methodology

### 1. Insertion
- Insert the new node following Binary Search Tree rules.
- Initially color the new node Red.
- Check for Red-Black Tree property violations.
- Apply recoloring and rotations when required.

### 2. Deletion
- Locate the node to be deleted.
- Delete it following BST deletion rules.
- Check whether the deletion violates Red-Black properties.
- Apply recoloring and rotations to restore balance.

### 3. Searching
- Start from the root node.
- Compare the search value with the current node.
- Move to the left subtree if the value is smaller.
- Move to the right subtree if the value is larger.
- Continue until the element is found or the search reaches a NIL node.

## Rotations

Rotations are structural operations used to maintain the balance of the tree.

### Left Rotation
A left rotation moves a node's right child upward and adjusts the corresponding subtree links.

### Right Rotation
A right rotation moves a node's left child upward and adjusts the corresponding subtree links.

These operations preserve the Binary Search Tree ordering.

## Time Complexity

| Operation | Time Complexity |
|---|---|
| Search | O(log n) |
| Insertion | O(log n) |
| Deletion | O(log n) |
| Traversal | O(n) |
| Left / Right Rotation | O(1) |

## Technologies Used
- Programming Language: C
- Data Structure: Red-Black Tree
- Concepts: Binary Search Tree, Structures, Pointers, Dynamic Memory Allocation, Recursion, Tree Rotations

## Key Concepts Learned
- Binary Search Tree operations
- Self-balancing tree concepts
- Red-Black Tree properties
- Left and right rotations
- Recoloring techniques
- Recursive tree operations
- Dynamic memory allocation
- Time complexity analysis

## Applications
- Database indexing
- Memory management
- Operating system implementations
- Associative containers
- Efficient searching and sorting systems

## How to Run

1. Clone the repository:

   ```bash
   git clone <repository-url>
   ```

2. Navigate to the project directory:

   ```bash
   cd <project-folder>
   ```

3. Compile the source files:

   ```bash
   gcc *.c -o red_black_tree
   ```

4. Execute the program:

   ```bash
   ./red_black_tree
   ```

*Modify the compilation command according to your actual source-file structure.*

## Future Improvements
- Visual representation of tree operations
- Improved input validation
- Support for additional tree traversal methods
- Performance testing with large datasets

## Conclusion
This project provides practical experience in implementing a self-balancing tree using C. It strengthens the understanding of Binary Search Trees, pointers, dynamic memory allocation, rotations, recoloring, and efficient data organization.

## Author
**Manjusha Thiruveedhula**
