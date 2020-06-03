# Prefix Dictionary Interface

## Learning Goals

By the end of this module, students will be able to...

- **Describe** how a T9 keyboard works
- **List** the important features of the prefix dictionary interface

## Lesson Content

# TODO PANOPTO

### Summary

We need a data structure to track associations between **codes** and **words**, both strings

Key operation: Lookup words by **code prefix**

Goals:

- Fast lookup (`\(O(c + m)\)` time for a code of length `\(c\)` resulting in `\(m\)` matches)
- Minimal storage space

Note: this is a little different than what was in the video

## Challenges

<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: 1b66e1f2-367d-48a0-9e92-23617d8c9a1c
* title: T9 Codes

##### !question

What is the T9 code for the word "algorithm"?

##### !end-question

##### !options

* 382294672
* 255872394
* 254674846
* 255546667774448446

##### !end-options

##### !answer

* 254674846

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
* id: c74f5f33-b907-45a9-afd3-88803bff3a4d
* title: Prefix Dictionary Records

##### !question

What kinds of records does a prefix dictionary store?

##### !end-question

##### !options

* Opaque elements
* Opaque keys and values
* String codes and string words
* Numeric codes and string words

##### !end-options

##### !answer

* String codes and words

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
* id: 346e0ae8-8068-4c3b-9e58-da19e57d2bc5
* title: Performance

##### !question

For which prefix dictionary operation do we care the **least** about performance?

##### !end-question

##### !options

* Lookup code
* Lookup prefix
* Insert a word
* None of the above

##### !end-options

##### !answer

* Insert a word

##### !end-answer

<!-- other optional sections -->
<!-- !hint - !end-hint (markdown, users can see after a failed attempt) -->
<!-- !rubric - !end-rubric (markdown, instructors can see while scoring a checkpoint) -->
<!-- !explanation - !end-explanation (markdown, students can see after answering correctly) -->

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
