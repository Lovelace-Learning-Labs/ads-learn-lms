# Trie Analysis

## Learning Goals

By the end of this module, students will be able to...

## Lesson Content

# TODO PANOPTO

### Summary

\\(c\\) is code length, \\(m\\) is number of matches

| Operation      | Time           | Space      |
| -------------- | -------------- | ---------- |
| Lookup code    | \\(O(c)\\)     | constant   |
| Lookup prefix  | \\(O(c + m)\\) | \\(O(m)\\) |
| Insert one     | \\(O(c)\\)     | constant   |
| Insert \\(n\\) | \\(O(n * c)\\) | \\(O(n)\\) |

Key takeaway: trie time complexity is **independent of the number of records**

## Challenges

<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: 55443484-74ba-4517-a6b7-495798013107
* title: Constant \\(k\\)

##### !question

What do we mean when we say that \\(k\\) (the average code length) is constant?

##### !end-question

##### !options

* \\(k\\) is the same for all tries
* \\(k\\) is the same for all tries of size \\(n\\)
* For a given trie, \\(k\\) stays the same as \\(n\\) grows

##### !end-options

##### !answer

* For a given trie, \\(k\\) stays the same as \\(n\\) grows

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
* id: 117377e3-a837-4dab-b78f-e0e1512a1f63
* title: Lookup Prefix

##### !question

What does the time complexity of `lookupPrefix` depend on?

##### !end-question

##### !options

* The number of nodes \\(n\\) in the trie
* The height \\(h\\) of the trie
* The length \\(c\\) of the prefix
* The average length \\(k\\) of a code in the trie
* The max length \\(max(k)\\) of a code in the trie
* The number of records \\(m\\) matching the prefix

##### !end-options

##### !answer

* The length \\(c\\) of the prefix
* The number of records \\(m\\) matching the prefix

##### !end-answer

<!-- other optional sections -->
<!-- !hint - !end-hint (markdown, users can see after a failed attempt) -->
<!-- !rubric - !end-rubric (markdown, instructors can see while scoring a checkpoint) -->
<!-- !explanation - !end-explanation (markdown, students can see after answering correctly) -->

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
