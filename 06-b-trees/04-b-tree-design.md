# B-Tree Design

## Learning Goals

By the end of this module, students will be able to...

- **Describe** the structure of a B-Tree node
- **Compare** the B-Tree property to the BST property
- **State** the height of a B-Tree in terms of the number of records

## Lesson Content

# TODO Panopto

## Summary

The **degree** \\(d\\) of a non-leaf node is its number of children. A node with \\(d\\) children stores \\(d-1\\) key-value pairs.

A B-Tree has **min degree** \\(t\\) and **max degree** \\(2t\\).

The **B-Tree property** is similar to the BST property:

>Let `node` be any non-leaf node. Then for each index \\(0 \leq i \lt d-1\\)...
>- All keys in the subtree at `node.children[i]` are less than `node.keys[i]`
>- All keys in the subtree at `node.children[i+1]` are greater than `node.keys[i]`

All **leaf nodes** have the same **depth**. This means that for a B-tree with \\(n\\) records, the height \\(h = O(log(n))\\).

## Challenges