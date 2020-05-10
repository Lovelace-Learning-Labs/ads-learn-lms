# BST Design

## Learning Objectives

By the end of this module, students will be able to...

- **Define** the terms linear search, binary search, binary search tree, root, parent, child, ancestor, descendant, subtree
- **Explain** why previously studied data structures aren't sufficient to implement a fast ordered dictionary
- **Use** binary search to find an element in a sorted array in `\(O(log(n))\)` time
- **Describe** the structure of a binary search tree

## Lesson Content

https://adaacademy.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=cd2e977a-e944-41f6-9886-abb70032b53c

## Challenges


<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: checkbox
* id: 68b5d338-6c15-4688-ab81-97ecec36b5ce
* title: Steal like an artist
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

Which of these features did we steal from other data structures for our binary search tree?

##### !end-question

##### !options

* Storing records in sorted order to allow `O(n)` iteration and `O(log(n))` lookup via binary search
* Storing records in insertion order to quickly find the oldest or newest record
* Using linked nodes to store records to enable quick random insert and delete
* Using a hash function to get constant-time lookup and insert
* Storing records in contiguous memory to promote cache hits on workflows with high locality

##### !end-options

##### !answer

* Storing records in sorted order to allow `O(n)` iteration and `O(log(n))` lookup via binary search
* Using linked nodes to store records to enable quick random insert and delete

##### !end-answer

<!-- other optional sections -->
<!-- !hint - !end-hint (markdown, users can see after a failed attempt) -->
<!-- !rubric - !end-rubric (markdown, instructors can see while scoring a checkpoint) -->
<!-- !explanation - !end-explanation (markdown, students can see after answering correctly) -->

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: 9fa45f9a-30e9-4eed-9bc1-342175d26269
* title: BST node links
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

How many links does each node contain in a binary search tree?

##### !end-question

##### !options

* 1
* 2
* 3
* 4

##### !end-options

##### !answer

* 3

##### !end-answer

##### !explanation

Each node has links to its left child, right child, and parent

##### !end-explanation

<!-- other optional sections -->
<!-- !hint - !end-hint (markdown, users can see after a failed attempt) -->
<!-- !rubric - !end-rubric (markdown, instructors can see while scoring a checkpoint) -->
<!-- !explanation - !end-explanation (markdown, students can see after answering correctly) -->

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: 006a5ea6-0968-48af-975b-0cb916b33111
* title: BST property
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

Which of the following is the binary search tree property?

##### !end-question

##### !options

* For every node, all keys at a lower level in the tree are less than its key, and all keys above it are greater
* For every node, all keys at a lower level in the tree are greater than its key, and all keys above it are less
* For every node, all keys in the left subtree are less than its key, and all keys in the right subtree are greater
* For every node, all keys in the left subtree are greater than its key, and all keys in the right subtree are less
* Every subtree is also a binary search tree
* A binary search tree must be balanced

##### !end-options

##### !answer

* For every node, all keys in the left subtree are less than its key, and all keys in the right subtree are greater

##### !end-answer

<!-- other optional sections -->
<!-- !hint - !end-hint (markdown, users can see after a failed attempt) -->
<!-- !rubric - !end-rubric (markdown, instructors can see while scoring a checkpoint) -->
<!-- !explanation - !end-explanation (markdown, students can see after answering correctly) -->

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: 791ba9c3-b570-4576-8cf8-643edd6eca5a
* title: Parents
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

How many nodes in a binary search tree have no parent?

##### !end-question

##### !options

* 0
* 1
* 2
* There is no limit on how many nodes may be without a parent

##### !end-options

##### !answer

* 1

##### !end-answer

##### !explanation

The root is the only node in the tree with no parent

##### !end-explanation

<!-- other optional sections -->
<!-- !hint - !end-hint (markdown, users can see after a failed attempt) -->
<!-- !rubric - !end-rubric (markdown, instructors can see while scoring a checkpoint) -->
<!-- !explanation - !end-explanation (markdown, students can see after answering correctly) -->

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: 130e4da5-d9ba-4060-b260-f157f2bc9103
* title: Subtrees
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

Select the best definition of a subtree

##### !end-question

##### !options

* All the nodes to either the left or the right of the root
* All the layers in a tree down to a certain level
* All the children of a node, its children's children, etc.
* A node and all of its descendants
* A node and all of its ascendants

##### !end-options

##### !answer

* A node and all of its descendants

##### !end-answer

<!-- other optional sections -->
<!-- !hint - !end-hint (markdown, users can see after a failed attempt) -->
<!-- !rubric - !end-rubric (markdown, instructors can see while scoring a checkpoint) -->
<!-- !explanation - !end-explanation (markdown, students can see after answering correctly) -->

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
