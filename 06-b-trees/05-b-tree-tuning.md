# B-Tree Tuning

## Learning Goals

By the end of this module, students will be able to...

* **Describe** the relationship between a B-Tree's minimum degree `\(t\)` and its height
* **Calculate** an optimal value of `\(t\)` for a given page size and record structure

## Lesson Content

# TODO Panopto

## Summary

The minimum degree \\(t\\) has a big impact on a B-Tree's structure and performance

Our goal is to select \\(t\\) to **minimize the number of pages read on a walk from the root to a leaf**

Idea: select \\(t\\) so that the **max size of a node** (\\(d=2t\\)) is as close to the **size of a page** as possible without going over

## Challenges

<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: d34cc989-62f6-4d6f-a1a0-0909078a19f6
* title: Minimum degree impact

##### !question

How does increasing the minimum degree \\(t\\) affect the structure of a B-Tree?

##### !end-question

##### !options

* A tree with the same number of nodes can hold more records
* A tree of the same height contains more nodes
* Both of the above
* None of the above

##### !end-options

##### !answer

* Both of the above

##### !end-answer

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: 47b1bfe4-b232-4bf5-a9c3-44c9b6b978c0
* title: Key size and \\(t\\)

##### !question

How does the size of a key affect \\(t\\)?

##### !end-question

##### !options

* Bigger keys mean smaller \\(t\\)
* Bigger keys mean bigger \\(t\\)
* Key size does not affect \\(t\\)

##### !end-options

##### !answer

* Bigger keys mean smaller \\(t\\)

##### !end-answer

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
