# Memory Swapping

## Learning Goals

By the end of this module, students will be able to...

- **Compare** main memory (RAM) with secondary memory (disk)
- **Explain** why memory is organized into pages
- **Describe** the technique of swapping memory to disk

## Lesson Content

<iframe src="https://adaacademy.hosted.panopto.com/Panopto/Pages/Embed.aspx?id=3f5b83e4-595c-4ae9-8067-abdc013db044&autoplay=false&offerviewer=true&showtitle=true&showbrand=false&start=0&interactivity=all" width=720 height=405 style="border: 1px solid #464646;" allowfullscreen allow="autoplay"></iframe>

## Summary

**Secondary memory** (disk) is 100x cheaper but 100,000x slower than **main memory** (RAM). Most computers have way more disk space than RAM.

Memory is organized into fixed-size **pages** of a few KB each. To boost performance, secondary memory is always read / written in page.

**Swapping** pages of main memory out to disk lets us pretend we have extra memory available.

### Additional Reading

If you want to learn more about secondary memory, you might find these resources interesting:

- [The B-Trees chapter in CLRS Intro to Algorithms](http://staff.ustc.edu.cn/~csli/graduate/algorithms/book6/chap19.htm) starts with a discussion of how disk drives work
- [Latency Numbers Every Programmer Should Know](https://gist.github.com/jboner/2841832)
- UW Madison has an [excellent free textbook on operating systems](http://pages.cs.wisc.edu/~remzi/OSTEP/) available online, including
    - [Intro to Virtual Memory and Paging](http://pages.cs.wisc.edu/~remzi/OSTEP/vm-paging.pdf)
    - [Intro to Disk Drives](http://pages.cs.wisc.edu/~remzi/OSTEP/file-disks.pdf)

## Challenges

<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: cdc83889-faa7-4391-8561-f84df479176e
* title: Main memory access time

##### !question

How would you measure the amount of time it takes for a computer to access a value stored in **main memory**?

##### !end-question

##### !options

* Milliseconds
* Microseconds
* Nanoseconds

##### !end-options

##### !answer

* Nanoseconds

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
* id: ba867495-9c30-4f6a-8e0c-31d9102f8c59
* title: Disk access time

##### !question

How would you measure the amount of time it takes for a computer to access a value stored on **disk**?

##### !end-question

##### !options

* Milliseconds
* Microseconds
* Nanoseconds

##### !end-options

##### !answer

* Milliseconds

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
* id: 4bd63b84-8a63-40d5-bca2-4b00a7ed1797
* title: Swapping

##### !question

What is the key idea behind memory swapping?

##### !end-question

##### !options

* Every time you write to main memory you also copy that data to disk, to ensure data persists through power loss
* Data lives on disk, and individual pages of memory are loaded into main memory as needed
* Memory swapping lets us improve the cost/speed tradeoff between main memory and secondary storage

##### !end-options

##### !answer

* Data lives on disk, and individual pages of memory are loaded into main memory as needed

##### !end-answer

<!-- other optional sections -->
<!-- !hint - !end-hint (markdown, users can see after a failed attempt) -->
<!-- !rubric - !end-rubric (markdown, instructors can see while scoring a checkpoint) -->
<!-- !explanation - !end-explanation (markdown, students can see after answering correctly) -->

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
