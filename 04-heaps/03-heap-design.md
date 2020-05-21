# Heap Design

## Learning Goals

By the end of this module, students will be able to...

* **Identify** features of other data structures relevant to implementing priority queues
* **Describe** how to lay out the nodes of a tree in an array
* **Recite** the max-heap property

## Lesson Content

# TODO Panopto

## Challenges

<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: e63b7df5-92ca-4ced-b928-29b4c298022c
* title: Heap parent
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

If a node in a heap is stored at index 7, at what index is its parent stored?

##### !end-question

##### !options

* 2
* 3
* 4
* 8
* 14

##### !end-options

##### !answer

* 3

##### !end-answer

##### !hint

A node's parent is at index \\( \lfloor{ i / 2 } \rfloor \\)

##### !end-hint

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->


<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: 6a32841d-37aa-4a27-ab4a-20988e736a81
* title: Heap children
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

If a node in a heap is stored at index 7, at what index is its parent stored?

##### !end-question

##### !options

* Left child at 13, right child at 14
* Left child at 14, right child at 15
* Left child at 15, right child at 16
* Left child at 14, right child at 13
* Left child at 15, right child at 14
* Left child at 16, right child at 15

##### !end-options

##### !answer

* Left child at 14, right child at 15

##### !end-answer

##### !hint

A node's left child is at index `\(2 * i\)`, and its right child at index `\(2 * i + 1\)`

##### !end-hint

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: 21dba7bd-4d74-4853-a663-504b7c6dfad2
* title: Heap identification A

##### !question

Is this a max-heap?

![](images/heap-identification-a.png)

##### !end-question

##### !options

* Yes
* No, it violates the max-heap property
* No, it's not perfectly balanced

##### !end-options

##### !answer

* No, it violates the max-heap property

##### !end-answer

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: 9a65266b-65b6-4d4b-9f3b-c1505593ba20
* title: Heap identification B

##### !question

Is this a max-heap?

![](images/heap-identification-b.png)

##### !end-question

##### !options

* Yes
* No, it violates the max-heap property
* No, it's not perfectly balanced

##### !end-options

##### !answer

* Yes

##### !end-answer

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: a00b8577-b08f-4254-a816-feec58cb5c4d
* title: Heap identification C

##### !question

Is this a max-heap?

![](images/heap-identification-c.png)

##### !end-question

##### !options

* Yes
* No, it violates the max-heap property
* No, it's not perfectly balanced

##### !end-options

##### !answer

* No, it's not perfectly balanced

##### !end-answer

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
