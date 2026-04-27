# Binary Trees

## Description

This project explores the concept of binary trees in C, covering their structure, traversal methods, and various properties. It progresses from simple binary trees to Binary Search Trees (BST), AVL Trees, and Max Binary Heaps.

## Learning Objectives

- Understand what a binary tree is and how it differs from a Binary Search Tree
- Gain/lose time complexity compared to linked lists
- Understand depth, height, and size of a binary tree
- Know the different traversal methods for binary trees
- Understand complete, full, perfect, and balanced binary trees

## Requirements

- **OS:** Ubuntu 20.04 LTS
- **Compiler:** `gcc` with flags `-Wall -Werror -Wextra -pedantic -std=gnu89`
- **Style:** Betty coding style
- **Editors:** `vi`, `vim`, `emacs`
- No global variables allowed
- No more than 5 functions per file
- All header files must be include-guarded

## Data Structures

/**
 * struct binary_tree_s - Binary tree node
 *
 * @n: Integer stored in the node
 * @parent: Pointer to the parent node
 * @left: Pointer to the left child node
 * @right: Pointer to the right child node
 */
struct binary_tree_s
{
    int n;
    struct binary_tree_s *parent;
    struct binary_tree_s *left;
    struct binary_tree_s *right;
};

typedef struct binary_tree_s binary_tree_t;


## Files

| File | Description |
|------|-------------|
| \`binary_trees.h\` | Header file with all prototypes and data structures |
| \`0-binary_tree_node.c\` | Creates a binary tree node |
| \`1-binary_tree_insert_left.c\` | Inserts a node as the left child |
| \`2-binary_tree_insert_right.c\` | Inserts a node as the right child |
| \`3-binary_tree_delete.c\` | Deletes an entire binary tree |
| \`4-binary_tree_is_leaf.c\` | Checks if a node is a leaf |
| \`5-binary_tree_is_root.c\` | Checks if a node is a root |
| \`6-binary_tree_preorder.c\` | Pre-order traversal |
| \`7-binary_tree_inorder.c\` | In-order traversal |
| \`8-binary_tree_postorder.c\` | Post-order traversal |
| \`9-binary_tree_height.c\` | Measures height of a binary tree |
| \`10-binary_tree_depth.c\` | Measures depth of a node |
| \`11-binary_tree_size.c\` | Measures size of a binary tree |
| \`12-binary_tree_leaves.c\` | Counts leaves in a binary tree |
| \`13-binary_tree_nodes.c\` | Counts nodes with at least one child |
| \`14-binary_tree_balance.c\` | Measures balance factor of a tree |
| \`15-binary_tree_is_full.c\` | Checks if a binary tree is full |
| \`16-binary_tree_is_perfect.c\` | Checks if a binary tree is perfect |
| \`17-binary_tree_sibling.c\` | Finds the sibling of a node |
| \`18-binary_tree_uncle.c\` | Finds the uncle of a node |

---
## Installation

1. Clone the repository:

git clone https://github.com/l44mz/holbertonschool-binary_trees.git

cd holbertonschool-binary_trees

2. Compile the project:

gcc -Wall -Werror -Wextra -pedantic -std=gnu89 -Wno-format *.c -o printf

---
## Usage Example

#include "binary_trees.h"


int main(void)
{

binary_tree_t *root;

root = binary_tree_node(NULL, 10);

binary_tree_insert_left(root, 5);

binary_tree_insert_right(root, 15);

return (0);

}

---
## Concepts

### Binary Tree Types

| Type | Description |
|------|-------------|
| **Full** | Every node has 0 or 2 children |
| **Complete** | All levels filled except possibly the last, filled left to right |
| **Perfect** | All internal nodes have 2 children; all leaves at same level |
| **Balanced** | Height of left and right subtrees differ by at most 1 |

### Traversal Methods

- **Pre-order:** Root → Left → Right
- **In-order:** Left → Root → Right
- **Post-order:** Left → Right → Root

## Authors

- Jana Alhazmi - GitHub: https://github.com/janaalhazmi
- Lama Almazroa - GitHub: https://github.com/l44mz

