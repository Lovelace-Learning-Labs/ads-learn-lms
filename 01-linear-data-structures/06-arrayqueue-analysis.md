# ArrayQueue Analysis

## Learning Objectives

By the end of this module, students will be able to...

- **Describe** the time and space complexity of each operation on our ArrayQueue
- **Analyze** the complexity of workflows
- **Explain** the reasoning behind an amortized complexity

## Lesson Content

https://adaacademy.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=b718a392-ab38-4557-8b56-abb40058a03d

## Challenges

<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: 0a03a901-d0ea-4a0c-ad94-dbf7bc78d42b
* title: Variable names
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

Where did the letters \\(c\\), \\(d\\) and \\(e\\), come from?

##### !end-question

##### !options

* Those are the traditional letters for those quantities
* Made up on the spot for convenience, using the first letter of what they describe
* Dan gazed upon the void that he might know that which is forbidden

##### !end-options

##### !answer

* Made up on the spot for convenience, using the first letter of what they describe

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
* id: dbbcd468-c1dd-43bc-a59a-2a95bd9f5bed
* title: Amortized definition
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

What does it mean for `dequeue` to be amortized constant time?

##### !end-question

##### !options


* It always runs in constant time
* It occasionally runs in constant time, as a best-case scenario
* The average run time over many dequeues is constant, but occasionally it may be much worse
* If time is constant then space is linear

##### !end-options

##### !answer

* The average run time over many dequeues is constant, but occasionally it may be much worse

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
* id: 4fb8d764-0751-4ba8-bb5f-102a168cf544
* title: Amortized conditions
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

In which of the following scenarios would dequeue not be amortized constant time?

Remember that \\(e\\) is the number of elements that have ever been enqueued.

##### !end-question

##### !options

* 1 cancel and \\(e - 1\\) dequeues
* 50% cancels and 50% dequeues
* \\(e - 1\\) cancels and 1 dequeue

##### !end-options

##### !answer

* \\(e - 1\\) cancels and 1 dequeue

##### !end-answer

##### !explanation

The math to figure out that dequeue is amortized constant relies on \\(d\\) being linear in terms of \\(e\\). In other words a constant portion of elements end up getting dequeued instead of canceled.

<br>

If that's true then we can "spread out" the cancels amongst the dequeues, and it will always work out to a constant number.

<br>

But if \\(d\\) is sub-linear (e.g. constant or logarithmic), then \\(c\\) (which must be linear, since it has to pick up all the leftover elements) grows faster, and the relationship breaks down. There's not enough dequeues to "soak up" all the cancels, and the more elements you add the worse the situation becomes.

<br>

The most extreme case of this is when \\(d\\) is a constant like 4. Then there's \\(e - d\\) cancels for each dequeue, which (since \\(d\\) is a constant) is \\(O(e)\\).

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
* id: 67f55273-5e31-4773-bffb-6428759c14a8
* title: Disappointment
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

At the end of the video, why are we unhappy with the performance of the ArrayQueue?

##### !end-question

##### !options

* Enqueue creates a new object on the heap but dequeue and cancel don't destroy it, creating a memory leak
* Enqueue increases the size of the storage array but dequeue and cancel don't decrease it, creating a memory leak
* Cancel is \\(O(n)\\) due to linear search for the element
* Dequeue has worst-case \\(O(c)\\) time complexity
* We're perfectly happy with the performance, thank you

##### !end-options

##### !answer

* Enqueue increases the size of the storage array but dequeue and cancel don't decrease it, creating a memory leak

##### !end-answer

<!-- other optional sections -->
<!-- !hint - !end-hint (markdown, users can see after a failed attempt) -->
<!-- !rubric - !end-rubric (markdown, instructors can see while scoring a checkpoint) -->
<!-- !explanation - !end-explanation (markdown, students can see after answering correctly) -->

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
