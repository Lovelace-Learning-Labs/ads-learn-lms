# ArrayQueue Implementation

## Learning Objectives

By the end of this module, students will be able to...

- **Define** the terms implementation, amortized
- **List** the important capabilities of JavaScript
- **Explain** how we'll use an array to implement the queue interface

## Lesson Content

<iframe src="https://adaacademy.hosted.panopto.com/Panopto/Pages/Embed.aspx?id=4bf8f2de-ca77-4244-bf71-abb4004fc218&autoplay=false&offerviewer=true&showtitle=true&showbrand=false&start=0&interactivity=all" width=720 height=405 style="border: 1px solid #464646;" allowfullscreen allow="autoplay"></iframe>

Some of these questions ask about the implementation of ArrayQueue. You can find that in this week's lab repo, under `src/data_structures/array_queue.js`.

## Challenges

<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: checkbox
* id: 260f9850-babf-4543-a15b-655e24282dff
* title: JavaScript Arrays
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

Which of the following are true of JavaScript arrays

##### !end-question

##### !options

* They resize themselves automatically
* Append is amortized constant time
* They can contain multiple types
* They are always backed by contiguous memory

##### !end-options

##### !answer

* They resize themselves automatically
* Append is amortized constant time
* They can contain multiple types

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
* id: 250764c5-eed6-48d6-a176-410b24652af6
* title: ArrayQueue cancelation
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

What does the ArrayQueue implementation use as a cancelation ticket?

##### !end-question

##### !options

* An md5 hash of the element
* The element's index in the storage array
* The element's address in memory
* The node containing the element

##### !end-options

##### !answer

* The element's index in the storage array

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
* id: 75aacba8-45c9-457e-950c-0f303f6d9d8b
* title: Dequeue implementation
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

What might happen if we removed the `while` loop at the start of `dequeue`?

##### !end-question

##### !options

* Nothing bad
* The `head` index might become greater than the `tail` index
* We might return a canceled element
* We might return `undefined` when there are still elements in the queue
* We might overwrite an existing element the next time

##### !end-options

##### !answer

* We might return `undefined` when there are still elements in the queue

##### !end-answer

<!-- other optional sections -->
<!-- !hint - !end-hint (markdown, users can see after a failed attempt) -->
<!-- !rubric - !end-rubric (markdown, instructors can see while scoring a checkpoint) -->
<!-- !explanation - !end-explanation (markdown, students can see after answering correctly) -->

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
