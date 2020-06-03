# Discussion Questions

## Tries

Please read through these before class, and come prepared to have a meaningful discussion with your peers

For each question we'll discuss in small groups, then as a big group

## General

1. Introduce yourself to your group!
1. What questions or comments do you have after watching the video lectures?
1. What is the height of a trie?
1. Would it be a good idea to use an array to store a trie like a heap? Why or why not?
1. Consider a trie where the codes are in binary (1s and 0s)
    - What is the branching factor for such a trie?
    - How would you generate codes?
    - How does this compare to a BST?
1. How could you optimize a trie if every word is its own code?
    - E.g. the words "ada", "developers" and "academy" would have the codes "ada", "developers" and "academy"
    - We call the mapping from a word to itself the "identity" mapping
1. How could you reduce the space used by a trie?
    - Hint: think about runs of inner nodes that don't store any words
    - What operations would need to change?
    - Does this change the time or space complexity of any operations?