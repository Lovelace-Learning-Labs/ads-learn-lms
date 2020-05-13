# Review: Algorithmic Analysis

## Learning Objectives

By the end of this module, students will be able to...

* **Define** the terms analysis, complexity, order, worst case
* **Explain** how Big-O notation helps compare algorithms
* **Recognize** the graph shapes of common complexity orders
* **Recall** the time complexity of various basic operations
* **Describe** how to compose operations to analyze the complexity of a function

## Lesson Content

This lesson is review! If you are confident you remember the basics of algorithmic analysis, feel free to skip to the comprehension questions.

https://adaacademy.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=91d8f64d-b37a-4b1f-b18a-abb3000f5703

## Challenges

<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: f76395b5-fd49-42a1-9188-0c6bb3332eb3
* title: Point of Big-O
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

What is the point of Big-O notation?

##### !end-question

##### !options

* Big-O gives us a relatively simple mathematical formula that behaves similar to our messy real-world performance
* Big-O allows us to make comparisons between different algorithms
* Big-O describes the performance of our algorithm in terms of the input
* All of the above

##### !end-options

##### !answer

* All of the above

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
* id: 3898afe3-237e-4a6d-852f-adbc0fe917ea
* title: `O(n)` meaning
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

Saying that an algorithm is \\(O(n)\\) is sufficient to analyze its growth

##### !end-question

##### !options

* Yes
* No, because we don't know what coefficient \\(n\\) might have
* No, because we haven't said what \\(n\\) is

##### !end-options

##### !answer

* No, because we haven't said what \\(n\\) is

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
* id: 479c892b-9e90-4fe7-8f40-9495bac6063c
* title: Growth - slower than input
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

Which of the following complexity orders grow **slower** than the input

##### !end-question

##### !options

* Constant - \\(O(1)\\)
* Logarithmic - \\(O(log(n))\\)
* Linear - \\(O(n)\\)
* Log-linear - \\(O(n*log(n))\\)
* Polynomial - \\(O(n^2)\\), \\(O(n^3)\\), etc

##### !end-options

##### !answer

* Constant - \\(O(1)\\)
* Logarithmic - \\(O(log(n))\\)

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
* id: e5f7afc1-cd0a-4811-9407-471b2f57f8c2
* title: Growth - same as input
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

Which of the following complexity orders grow **at the same rate** as the input

##### !end-question

##### !options

* Constant - \\(O(1)\\)
* Logarithmic - \\(O(log(n))\\)
* Linear - \\(O(n)\\)
* Log-linear - \\(O(n*log(n))\\)
* Polynomial - \\(O(n^2)\\), \\(O(n^3)\\), etc

##### !end-options

##### !answer

* Linear - \\(O(n)\\)

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
* id: 94551b01-1086-487c-954e-3288a517f8a7
* title: Growth - faster than input
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

Which of the following complexity orders grow **at the same rate** as the input

##### !end-question

##### !options

* Constant - \\(O(1)\\)
* Logarithmic - \\(O(log(n))\\)
* Linear - \\(O(n)\\)
* Log-linear - \\(O(n*log(n))\\)
* Polynomial - \\(O(n^2)\\), \\(O(n^3)\\), etc

##### !end-options

##### !answer

* Log-linear - \\(O(n*log(n))\\)
* Polynomial - \\(O(n^2)\\), \\(O(n^3)\\), etc

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
* id: b0b6e009-590d-46a7-98f2-f3a4d5d0b47c
* title: Analysis focus
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

Unless otherwise stated, which of the following do we typically analyze?

##### !end-question

##### !options

* The worst-case performance of an algorithm
* The average performance of an algorithm
* The best-case performance of an algorithm

##### !end-options

##### !answer

* The worst-case performance of an algorithm

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
* id: d4b06e41-ef40-44c6-b55d-da12c3ac35f5
* title: Analysis
<!-- * points: [1] (optional, the number of points for scoring as a checkpoint) -->
<!-- * topics: [python, pandas] (optional the topics for analyzing points) -->

##### !question

If \\(n\\) is the size of the input array, what is the time complexity of the following algorithm?

```js
// Stop words are common words that don't add semantic meaning to a text
// Natural langugage algorithms commonly filter them out as a first step
// Here we're counting them instead of filtering
const countStopWords = (words) => {
  const stopWords = {
    'a': 0,
    'the': 0,
    'are': 0,
    'and': 0, 
    'of': 0
  };
  words.forEach(word => {
    Object.keys(stopWords).forEach(stopWord => {
      if (word === stopWord) {
        stopWords[word] += 1;
      }
    });
  });
  return stopWords;
}
```

##### !end-question

##### !options

* \\(O(1)\\)
* \\(O(log(n))\\)
* \\(O(n)\\)
* \\(O(n^2)\\)

##### !end-options

##### !answer

* \\(O(n)\\)

##### !end-answer

##### !hint

Even though this code contains a nested loop, the inner loop runs a fixed number of times that doesn't grow with the size of the input array.

##### !end-hint

<!-- other optional sections -->
<!-- !hint - !end-hint (markdown, users can see after a failed attempt) -->
<!-- !rubric - !end-rubric (markdown, instructors can see while scoring a checkpoint) -->
<!-- !explanation - !end-explanation (markdown, students can see after answering correctly) -->

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
