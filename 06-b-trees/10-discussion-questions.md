# Discussion Questions

## B-Trees

Please read through these before class, and come prepared to have a meaningful discussion with your peers

For each question we'll discuss in small groups, then as a big group

## General

1. Introduce yourself to your group!
1. What questions or comments do you have after watching the video lectures?
1. We typically consider the minimum value for \\(t\\) (the "minimum minimum degree") to be 2. Why?
    - Hint: what is a B-Tree with minimum degree 1? How does this affect balance?
1. For a B-Tree with minimum degree \\(t\\) and height \\(h\\), what is the...
    - Minimum number of nodes
    - Maximum number of nodes
    - Minimum number of records
    - Maximum number of records
    - Use your equations to compare B-Trees with minimum degree of 10 vs 20
1. Describe the data structure that would result if each black node in a red-black tree were to absorb its red children, incorporating their children with its own.
1. How would you design a B-Tree to handle variable-sized keys like strings?
1. Could you increase the number of records stored in a leaf node? How would you determine how many records to store?
1. Suppose that we insert the keys `[1, 2, 3 ... n]` in order into an empty B-Tree with minimum degree two. How many nodes does the final B-Tree have?