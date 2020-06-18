# B-Tree Implementation

## Learning Goals

By the end of this module, students will be able to...

## Lesson Content

<iframe src="https://adaacademy.hosted.panopto.com/Panopto/Pages/Embed.aspx?id=d341a60a-54c2-4327-a501-abdd013996e2&autoplay=false&offerviewer=true&showtitle=true&showbrand=false&start=0&interactivity=all" width=720 height=405 style="border: 1px solid #464646;" allowfullscreen allow="autoplay"></iframe>

## Summary

Lookup is similar to BST lookup.

Insert is more complicated because we split full nodes. We split preemptively to avoid backtracking. Insert keeps the B-Tree balanced.

| Operation | Time              | Space      | Disk Accesses             |
| --------- | ----------------- | ---------- | ------------------------- |
| Lookup    | \\(O(log(n))\\)   | \\(O(t)\\) | \\(O(log(n))\\) (minimal) |
| Insert    | \\(O(t*log(n))\\) | \\(O(t)\\) | \\(O(log(n))\\) (minimal) |

Iterate (implementation and analysis) is up to you!

### Lookup Pseudocode

```ruby
def findIndex(node, key)
  # TODO upgrade to binary search
  i = 0
  while i < node.keys.length and node.keys[i] < key
    i += 1
  return i

def lookup(key)
  node = root

  while true
    i = findIndex(node, key)

    if i < node.keys.length and node.keys[i] == key
      return node.values[i]
    elsif node.isLeaf
      return undefined
    else
      node = node.children[i]
```

### Insert Pseudocode

```ruby
def splitChild(node, i)
  # TODO

def insert(key, value)
  if root.degree == 2 * t
    newRoot = new Node(isLeaf: false, children: [root])
    splitChild(newRoot, 0)
    root = newRoot

  node = root
  while true
    index = findIndex(node, key)
    if node.isLeaf
      node.keys.insertAt(index, key)
      node.values.insertAt(index, value)
      break

    else
      child = node.children[index]

      if child.degree == 2 * t
        splitChild(node, index)
        if key > node.keys[index]
          child = node.children[index + 1]

      node = child
```

## Challenges

<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: c616800b-c19f-41b9-b70b-16066c703f0c
* title: Non-leaf Records

##### !question

How does a record end up in a non-leaf node in a B-Tree?

##### !end-question

##### !options

* It was inserted directly into the non-leaf node
* It was originally inserted in a leaf and then "promoted" up the tree by a split by a later insert
* Either of the above
* Some other way

##### !end-options

##### !answer

* It was originally inserted in a leaf and then "promoted" up the tree by a split by a later insert

##### !end-answer

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: 2400a750-0ccd-4753-8cab-59abe772c49c
* title: Insert Progress

##### !question

Draw the results of inserting the keys

```
F, S, Q, K, C, L, H, T, V, W, M, R, N, P, A, B, X, Y, D, Z, E
```

in order into an empty B-Tree with minimum degree 2. Draw only the configurations of the tree just before some node must split, and also draw the final configuration.

> From CLRS Introduction to Algorithms, 2009

Use the [B-Tree visualizer](https://www.cs.usfca.edu/~galles/visualization/BTree.html) to check your work - make sure to set Max Degree to 4 and check "Preemptive Split".

##### !end-question

##### !options

* I did it!
* I didn't do it :(

##### !end-options

##### !answer

* I did it!

##### !end-answer

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
