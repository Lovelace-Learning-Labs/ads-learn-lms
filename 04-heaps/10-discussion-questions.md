# Discussion Questions

## Heaps

Please read through these before class, and come prepared to have a meaningful discussion with your peers

For each question we'll discuss in small groups, then as a big group

## General

1. Introduce yourself to your group!
1. What questions or comments do you have after watching the video lectures?
1. Is it possible for a tree to satisfy both the BST property and the max-heap property? Give an example or explain why not.
1. For a heap of height \\(h\\), what is the...
    - Maximum number of nodes
    - Maximum number of leaf nodes
    - Minimum number of nodes
    - Minimum number of leaf nodes
    - How are these numbers related to each other?
1. The video lesson describes the layout of a 1-indexed heap, with a null value at array index 0. This question asks you to consider a 0-indexed heap.
    - What equations could you use to find the parent and left/right child indices for a heap node at index \\(i\\)?
    - What advantage might there be to using a 1-indexed heap?
1. The interface for `heapsort` makes a lot of assumptions about the user's data. What are some of these assumptions, and how would you need to adjust your code to relax them?
1. In class we discussed max-heaps. Min-heaps also exist, they're the same except for the record with minimum priority is what gets removed. How would you need to change your heap implementation to get a min-heap?
1. Could you implement the sort part of the heapsort algorithm faster than \\(O(n*log(n))\\) if you had a second array to copy values into? Why or why not?
1. How would you delete an arbitrary node from a heap?
    - Make sure that you maintain the heap's balance and the max-heap property.
    - What is the runtime of your implementation? (Hint: it can be done in \\(O(log(n))\\) time)
    - How would the client tell you which node to remove?
1. A \\(b\\)-heap is a heap where non-leaf nodes have \\(b\\) children.
    - How would you lay out a \\(b\\)-heap in an array?
    - What is the height of a \\(b\\)-heap of size \\(n\\), in terms of \\(n\\) and \\(b\\)?
    - How would you implement `insert` on a \\(b\\)-heap?
        - What is the time complexity of this operation, in terms of \\(n\\) and \\(b\\)?
    - How would you implement `removeMax` on a \\(b\\)-heap?
        - What is the time complexity of this operation, in terms of \\(n\\) and \\(b\\)?