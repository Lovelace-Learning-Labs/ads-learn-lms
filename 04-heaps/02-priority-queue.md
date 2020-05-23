# Priority Queue Interface

## Learning Goals

By the end of this module, students will be able to...

- **Describe** the operations of the priority queue interface
- **List** the additional constraints we've added for this week
- **Differentiate** between queues and priority queues

## Lesson Content

# TODO Panopto

## Summary

A **priority queue** associates a priority with each stored record

Records are removed from the queue in priority order

We have added two constraints:

* Fixed maximum capacity
* No allocations after initialization

## Challenges

<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: 4ec51198-ddba-4a18-8880-78e44706b16b
* title: Priority queue records

##### !question

What kinds of records does our priority queue interface store?

##### !end-question

##### !options

* Opaque elements
* Opaque elements, each with a priority
* Key-value pairs
* Something else

##### !end-options

##### !answer

* Opaque elements, each with a priority

##### !end-answer

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: f3d537bf-aed4-4ef9-b1da-4324c728cd44
* title: Priority queue performance

##### !question

For a priority queue of capacity \\(c\\) storing \\(n\\) records, what performance do we require for `insert` and `removeMax`?

##### !end-question

##### !options

* \\(O(log(c))\\)
* \\(O(log(n))\\)
* \\(O(c)\\)
* \\(O(n)\\)

##### !end-options

##### !answer

* \\(O(log(n))\\)

##### !end-answer

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: 817a24f5-f692-4889-a4ec-176e9db8202d
* title: Allocation rules

##### !question

In which of the following methods will we be allowed to create new objects?

##### !end-question

##### !options

* The constructor
* `insert`
* `removeMax`
* None of the above

##### !end-options

##### !answer

* The constructor

##### !end-answer

##### !hint

The priority queue cannot allocate memory on the heap _after_ initialization. During the constructor is fine.

##### !end-hint

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
