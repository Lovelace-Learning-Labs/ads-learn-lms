# Rebalance

## Learning Objectives

By the end of this module, students will be able to...

- **Define** the terms red-black tree, rebalance, black-depth, rotation, induction
- **Explain** how, by following a set of rules, red-black trees can keep themselves balanced as they grow
- **Describe** the algorithm to rebalance a red-black tree after an insert

## Lesson Content

<iframe src="https://adaacademy.hosted.panopto.com/Panopto/Pages/Embed.aspx?id=8e9c3609-1cae-4b7b-bf9b-abbb0002c3ca&autoplay=false&offerviewer=true&showtitle=true&showbrand=false&start=0&interactivity=all" width=720 height=405 style="border: 1px solid #464646;" allowfullscreen allow="autoplay"></iframe>

## Challenges


<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: paragraph
* id: 1fc2285e-57db-4a75-ad2d-f455a8815242
* title: RBT rules
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

Describe in your own words how we know that a tree that follows the red-black tree rules is a balanced binary search tree.

##### !end-question

##### !placeholder

Your response...

##### !end-placeholder

<!-- other optional sections -->
<!-- !hint - !end-hint (markdown, users can see after a failed attempt) -->
<!-- !rubric - !end-rubric (markdown, instructors can see while scoring a checkpoint) -->
<!-- !explanation - !end-explanation (markdown, students can see after answering correctly) -->

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: paragraph
* id: 2296cb25-5b02-407e-803c-b8482cc3c7d5
* title: Induction
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

Describe in your own words why we can assume that a red-black tree is balanced before doing an insert.

##### !end-question

##### !placeholder

Your response...

##### !end-placeholder

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
* id: 309c5abf-7322-499a-ac8c-98c8c31717c5
* title: Rebalance complexity
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

Does adding a `rebalance` step to our `insert` change `insert`'s time complexity?

##### !end-question

##### !options

* No, because `rebalance` is constant-time
* No, because `rebalance` is \\(O(h)\\) time, same as `insert`
* No, because `rebalance` is \\(O(n)\\) time, same as `insert`
* Yes, it changes its complexity order

##### !end-options

##### !answer

* No, because `rebalance` is \\(O(h)\\) time, same as `insert`

##### !end-answer

<!-- other optional sections -->
<!-- !hint - !end-hint (markdown, users can see after a failed attempt) -->
<!-- !rubric - !end-rubric (markdown, instructors can see while scoring a checkpoint) -->
<!-- !explanation - !end-explanation (markdown, students can see after answering correctly) -->

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
