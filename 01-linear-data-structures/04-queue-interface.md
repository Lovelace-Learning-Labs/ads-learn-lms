# Queue Interface

## Learning Objectives

By the end of this module, students will be able to...

* **Define** the term interface and related keywords
* **Identify** questions to ask when designing an interface
* **Describe** the interface of a queue
* **Differentiate** between queries and commands

## Lesson Content

<iframe src="https://adaacademy.hosted.panopto.com/Panopto/Pages/Embed.aspx?id=9c6d03be-87b4-4884-8555-abb30039ecb7&autoplay=false&offerviewer=true&showtitle=true&showbrand=false&start=0&interactivity=all" width=720 height=405 style="border: 1px solid #464646;" allowfullscreen allow="autoplay"></iframe>

The `dll_queue.js` interface reviewed in the lecture lives here:

https://github.com/Lovelace-Learning-Labs/ads-linear-data-structures/blob/master/src/data_structures/dll_queue.js

## Challenges

<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: checkbox
* id: ac18876a-10d0-4f7b-9500-aaa7970bedd9
* title: Interface considerations
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

Which of the following are things we should consider when talking about an interface?

##### !end-question

##### !options

* What types of records are being stored
* How records will be organized in memory
* How client code will interact with the data structure
* Whether operations are queries or commands
* How specific operations will be implemented
* What patterns might appear in client workflows
* Any specific performance requirements

##### !end-options

##### !answer

* What types of records are being stored
* How client code will interact with the data structure
* Whether operations are queries or commands
* What patterns might appear in client workflows
* Any specific performance requirements

##### !end-answer

##### !hint

Remember, an interface describes what a data structure looks like from the outside.

* What is being stored?
* What operations can you do on stored data?
* What use patterns are best supported?

In addition, an interface might make guarantees about specific operations:

* This operation won't change stored data
* This operation will take at most this much time

An interface does **not** describe how things work "under the hood":

* The way records are stored in memory
* How an operation might be implemented

##### !end-hint

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
* id: e16199f7-67da-4379-a62b-66318dd57855
* title: Queue records
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question


What type of records does the queue interface store?

##### !end-question

##### !options

* Individual elements
* Key-value pairs
* JSON documents
* None of the above

##### !end-options

##### !answer

* Individual elements

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
* id: 80303c50-e61a-4679-9a10-e11563a8c4f1
* title: Dequeue order
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question


In what order are elements dequeued from a queue?

##### !end-question

##### !options

* Alphabetical
* Newest first
* Oldest first
* Order doesn't matter

##### !end-options

##### !answer

* Oldest first

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
* id: 5b9f7fad-b46f-485e-8a8d-4755d3e08c6d
* title: Cancelation
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

How is an element canceled from a queue?

##### !end-question

##### !options

* The client passes in the element to cancel
* The client passes in a cancelation ticket, an opaque object returned from enqueue
* The client passes in the index of the element
* The newest element is canceled

##### !end-options

##### !answer

* The client passes in a cancelation ticket, an opaque object returned from enqueue

##### !end-answer

<!-- other optional sections -->
<!-- !hint - !end-hint (markdown, users can see after a failed attempt) -->
<!-- !rubric - !end-rubric (markdown, instructors can see while scoring a checkpoint) -->
<!-- !explanation - !end-explanation (markdown, students can see after answering correctly) -->

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
