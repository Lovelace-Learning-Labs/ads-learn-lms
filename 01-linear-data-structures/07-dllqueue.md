# DLLQueue Implementation and Analysis

## Learning Objectives

By the end of this module, students will be able to...

- **Define** the following terms: linked list, node, head, tail, sentinel
- **Describe** the structure of a linked list
- **Describe** the implementation of various linked list operations
- **Discuss** the role of a sentinel node in a linked list
- **Use** a linked list to implement the queue interface

## Lesson Content

Part A: https://adaacademy.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=c312232b-3058-426b-bff0-abb500ee930b

Part B: https://adaacademy.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=f12295fb-2b79-457e-a665-abb500f5b887

## Challenges

<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: 013ee8b9-d0bc-4e4a-9437-461a20473d7a
* title: Doubly-linked list order
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question


How is order maintained between linked list nodes?

##### !end-question

##### !options

* They're stored in order in memory
* They're allocated randomly on the heap, so order isn't guaranteed
* A chain of references leads from node to the next in order

##### !end-options

##### !answer

* A chain of references leads from node to the next in order

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
* id: d93a2cb9-1bdc-443c-beba-e266400d5c6d
* title: Single vs double
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

Which operations are more difficult on a singly-linked list than a doubly-linked list?

##### !end-question

##### !options

* Insert head
* Insert tail
* Remove head
* Remove tail
* Remove by node
* Remove by element
* Iterate

##### !end-options

##### !answer

* Remove by node

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
* id: da9b6a78-d29a-4f89-96ac-bf2667d56b1c
* title: Sentinel node
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

What is the point of using a sentinel node?

##### !end-question

##### !options

* Provides invariants to keep our implementation simpler
* You can't make a doubly-linked list without one
* Prevents memory leaks on remove
* Prevents double-removing a node
* Allows reverse iteration

##### !end-options

##### !answer

* Provides invariants to keep our implementation simpler

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
* id: 4d2ab404-603c-4f82-a7e0-3e9d0610ddec
* title: [text, a short question title]
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

What does our DLLQueue return from enqueue as a cancelation ticket?

##### !end-question

##### !options

* The element's order in the queue
* The newly added node
* The node in front of the newly added node
* The element's memory address
* You can't cancel from a DLLQueue

##### !end-options

##### !answer

* The newly added node

##### !end-answer

<!-- other optional sections -->
<!-- !hint - !end-hint (markdown, users can see after a failed attempt) -->
<!-- !rubric - !end-rubric (markdown, instructors can see while scoring a checkpoint) -->
<!-- !explanation - !end-explanation (markdown, students can see after answering correctly) -->

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
