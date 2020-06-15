# B-Tree Tuning

## Learning Goals

By the end of this module, students will be able to...

* **Describe** the relationship between a B-Tree's minimum degree `\(t\)` and its height
* **Calculate** an optimal value of `\(t\)` for a given page size and record structure

## Lesson Content

# TODO Panopto

## Summary

The minimum degree `\(t\)` has a big impact on a B-Tree's structure and performance

Our goal is to select `\(t\)` to **minimize the number of pages read on a walk from the root to a leaf**

Idea: select `\(t\)` so that the **max size of a node** (`\(d=2t\)`) is as close to the **size of a page** as possible without going over

## Challenges