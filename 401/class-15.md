# Trees Cheatsheet

[Code Fellows Trees Tutorial](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)

## Terminology

- **Node**: A single data element in a tree.
- **Root**: The topmost node in a tree.
- **Edge**: A link between a parent node and a child node.
- **Child**: A node directly connected to another node when moving away from the root.
- **Parent**: The converse notion of a child.
- **Siblings**: Nodes with the same parent.
- **Leaf**: A node with no children.
- **Height**: The height of a tree is the number of edges from the tree's root to the furthest leaf.

## Types of Trees

- **Trees**: A non-linear data structure that contains a set of connected nodes with a hierarchical structure.
- **K-ary Trees**: A tree with any number of children possible (K represents the maximum number of children).
- **Binary Trees**: A tree in which each node can have at most two children.
- **Binary Search Trees (BST)**: A binary tree with the property that the values of the nodes to the left are less than or equal to the root node's value, and the values of the nodes to the right are greater than the root node's value.

## Traversals

- **Depth First Traversal**: A traversal method that explores the depth of a branch before moving on to another branch.
  - **Pre-order**: Root > Left > Right
  - **In-order**: Left > Root > Right (for BSTs, this results in sorted output)
  - **Post-order**: Left > Right > Root
- **Breadth First Traversal**: A traversal method that explores each level of the tree before moving on to the next level (also known as level-order traversal).

## Adding a Node to a Binary Search Tree

1. Start at the root node.
2. If the new value is less than the current node's value, go left.
3. If the new value is greater than the current node's value, go right.
4. If the next node in the chosen direction is `null`, insert the new node here.

## Big O

- Time complexity for inserting:
  - Worst case: O(n) (unbalanced tree)
  - Best case: O(log n) (balanced tree)
  - Average case: O(log n)
- Space complexity for inserting:
  - O(1)
- Time complexity for searching:
  - Worst case: O(n) (unbalanced tree)
  - Best case: O(log n) (balanced tree)
  - Average case: O(log n)
- Space complexity for searching:
  - Worst case: O(n) (unbalanced tree with recursive search)
  - Best case: O(1)
  - Average case: O(log n) (balanced tree with recursive search)
