# BST Implementation and Analysis

## Learning Objectives

By the end of this module, students will be able to...

- **Define** the terms depth, leaf, balanced, height, expected, pathological
- **Identify** whether a tree is balanced or unbalanced
- **Describe** the time and space complexity of tree operations
- **Explain** why it's important to keep a BST balanced

## Lesson Content

Note: this lesson was recorded before we decided to split BSTs and Red-Black Trees into separate weeks. As a result, some of the references to later modules might not make sense.

https://adaacademy.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=cc5c4864-27a8-464d-8e7f-abb7017d750a

### Recursion Review

This lesson relies on **recursion**. It's not the main focus, but it does come up in our discussion of `forEach`. If you're feeling nervous about recursion, you may wish to review Ada's CS Fun curriculum on recursion:

**Functions and the call stack**

- [Textbook page](https://github.com/Ada-Developers-Academy/textbook-curriculum/blob/master/04-cs-fundamentals/classroom/function-calls.md)
- [Video lesson](https://adaacademy.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=3ae487ad-99fc-41fd-ba79-aad60060e313)

**Writing recursive functions**

- [Textbook page](https://github.com/Ada-Developers-Academy/textbook-curriculum/blob/master/04-cs-fundamentals/classroom/recursion.md)
- [Video lesson](https://adaacademy.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=5250fb87-0391-438b-a492-aaed0018dc67)


## Challenges


<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: 802ee378-41dc-4858-b088-728c7e86a89b
* title: Balance
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

Select the best definition for **balanced**

##### !end-question

##### !options

* A tree is balanced if all nodes have the same depth
* A tree is balanced if all leaves have the same depth
* A tree is balanced if no node is more than twice as deep as any other
* A tree is balanced if no leaf is more than twice as deep as any other

##### !end-options

##### !answer

* A tree is balanced if no leaf is more than twice as deep as any other

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

* type: checkbox
* id: 88e28696-e434-42dc-a269-7633133659d3
* title: Balance and height
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

If `n` is the number of records in the tree, which of the following statements are true?

##### !end-question

##### !options

* The height of a balanced tree is `O(log(n))`
* The height of a balanced tree is `O(n)`
* The height of an unbalanced tree is `O(log(n))`
* The height of an unbalanced tree is `O(n)`

##### !end-options

##### !answer

* The height of a balanced tree is `O(log(n))`
* The height of an unbalanced tree is `O(n)`

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
* id: 1b7ce879-a71b-4240-99f2-1e5f5ef23a11
* title: Pathological input
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

Which of the following statements is true?

##### !end-question

##### !options

* Sorted input is pathological for a BST, because it creates a perfectly balanced tree
* Sorted input is pathological for a BST, because it creates an unbalanced tree
* Randomly ordered input is pathological for a BST, because it creates a perfectly balanced tree
* Randomly ordered input is pathological for a BST, because it creates an unbalanced tree

##### !end-options

##### !answer

* Sorted input is pathological for a BST, because it creates an unbalanced tree

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

* type: checkbox
* id: 0ad5085a-0a37-43b0-8124-36112fb05a21
* title: BST complexity
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

If `n` is the number of records and `h` is the height of the tree, which of the following statements are true?

##### !end-question

##### !options

* Lookup, insert and delete takes `O(log(n))` time
* Lookup, insert and delete takes `O(n)` time
* Lookup, insert and delete takes `O(log(h))` time
* Lookup, insert and delete takes `O(h)` time
* Iterate takes `O(log(n))` time
* Iterate takes `O(n)` time
* Iterate takes `O(log(h))` time
* Iterate takes `O(h)` time
* Iterate takes `O(log(n))` space
* Iterate takes `O(n)` space
* Iterate takes `O(log(h))` space
* Iterate takes `O(h)` space

##### !end-options

##### !answer

* Lookup, insert and delete takes `O(h)` time
* Iterate takes `O(n)` time
* Iterate takes `O(h)` space

##### !end-answer

<!-- other optional sections -->
<!-- !hint - !end-hint (markdown, users can see after a failed attempt) -->
<!-- !rubric - !end-rubric (markdown, instructors can see while scoring a checkpoint) -->
<!-- !explanation - !end-explanation (markdown, students can see after answering correctly) -->

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
