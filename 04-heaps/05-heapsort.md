# Heapsort

## Learning Goals

By the end of this module, students will be able to...

- **Explain** how to build a heap from an unsorted list
- **Demonstrate** how to turn a max-heap into a sorted array
- **Express** the time and space complexity of heapsort in big-O notation
- **Compare** heapsort to other sorting algorithms

## Lesson Content

## TODO Panopto link

### Summary

Heapsort is a pretty good sorting algorithm

Steps to sort an array of size \\(n\\):


* Build a heap from an unordered array: \\(O(n)\\) (woah!)
* Sort the heap using `removeMax`: \\(O(n*log(n))\\)
* **Total time complexity:** \\(O(n*log(n))\\)
* In-place, unstable


Quicksort does better on most inputs, but heapsort is a good fallback

## Challenges

<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: a6537358-639b-4898-aac8-11b8ebba33b7
* title: Buildheap complexity

##### !question

What is the time complexity of building a heap out of an unsorted array of size \\(n\\)?

##### !end-question

##### !options

* \\(O(log(n))\\)
* \\(O(n)\\)
* \\(O(n * log(n))\\)
* \\(O(n^2)\\)

##### !end-options

##### !answer

* \\(O(n)\\)

##### !end-answer

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: 1fdde984-0acb-446b-94af-e69e826796ac
* title: Heapsort time complexity

##### !question

What is the time complexity of the heapsort algorithm on an array of size \\(n\\)?

##### !end-question

##### !options

* \\(O(log(n))\\)
* \\(O(n)\\)
* \\(O(n*log(n))\\)
* \\(O(n^2)\\)

##### !end-options

##### !answer

* \\(O(n*log(n))\\)

##### !end-answer

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: fae630a1-e47b-4ed7-a352-7b7c26f1bb71
* title: Heapsort vs Mergesort

##### !question

What is the main advantage of heapsort over mergesort?

##### !end-question

##### !options

* Mergesort's average-case time complexity is worse than heapsort's
* Mergesort's worst-case time complexity is worse than heapsort's
* They have the same time complexity, but in practice heapsort is faster on most inputs
* Heapsort is in-place, but mergesort requires \\(O(n)\\) space

##### !end-options

##### !answer

* Heapsort is in-place, but mergesort requires \\(O(n)\\) space

##### !end-answer

##### !hint

Mergesort is not in-place

##### !end-hint

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: f781a3af-e54e-4bbd-a202-965645bfde16
* title: Heapsort vs Quicksort

##### !question

What is the main advantage of heapsort over quicksort?

##### !end-question

##### !options

* Quicksort's average-case time complexity is worse than heapsort's
* Quicksort's worst-case time complexity is worse than heapsort's
* They have the same time complexity, but in practice heapsort is faster on most inputs
* Heapsort is in-place, but quicksort requires \\(O(n)\\) space

##### !end-options

##### !answer

* Quicksort's worst-case time complexity is worse than heapsort's

##### !end-answer

##### !hint
Quicksort has \\(O(n^2)\\) time complexity on pathological input
##### !end-hint

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: f0356ece-879b-4a99-b29a-26d17cb12f9a
* title: System sort

##### !question

Which sorting algorithm is being used when you call `Array.sort`?

##### !end-question

##### !options

* Heapsort
* Mergesort
* Quicksort, possibly with a fallback to heapsort in the worst case

##### !end-options

##### !answer

* Quicksort, possibly with a fallback to heapsort in the worst case

##### !end-answer

<!-- other optional sections -->
<!-- !hint - !end-hint (markdown, users can see after a failed attempt) -->
<!-- !rubric - !end-rubric (markdown, instructors can see while scoring a checkpoint) -->
<!-- !explanation - !end-explanation (markdown, students can see after answering correctly) -->

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
