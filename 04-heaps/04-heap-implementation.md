# Heap Implementation

## Learning Goals

By the end of this module, students will be able to...

## Lesson Content

# TODO Panopto link

### Summary

To stay balanced, a heap must always **add and remove slots at the end** of the current storage, even if the record to add or remove doesn't go at the end.

We described **float** and **sink** subroutines to help us:

* **Insert:** add the record at the end, then "float" it up to the right spot by repeatedly swapping with its parent
* **Remove-Max:** swap root with the last element, then "sink" the new root down to the right spot by repeatedly swapping with its largest child

Pseudocode for sink and float:

#### Float

```ruby
def float(i)
  # Note: i and p are indices (not records)
  p = parent(i)
  while inBounds(p) && priority(p) < priority(i)
    swap(i, p)

    i = p
    p = parent(i)
```

#### Sink

```ruby
def sink(i)
  # Note: i, l, r and max are all indices (not records)
  finished = false
  until finished
    l = left(i)
    r = right(i)

    max = i
    if inBounds(l) && priority(l) > priority(max)
      max = l
    if inBounds(r) && priority(r) > priority(max)
      max = r

    if max == i
      finished = true
    else
      swap(i, max)
      i = max
```

## Challenges

<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: b5de383e-94bc-4dd1-8296-ddb3fbfdb096
* title: Insert Strategy

##### !question

Which of the following describes the strategy for inserting a record into a max-heap?

##### !end-question

##### !options

* Use linear search to find the space to insert
* Use binary search to find the space to insert
* Insert at the end of the storage array, then "float" the record up to the right place by repeatedly swapping with its parent
* Insert at the root, then "sink" the record down to the right place by repeatedly swapping with its larger child

##### !end-options

##### !answer

* Insert at the end of the storage array, then "float" the record up to the right place by repeatedly swapping with its parent

##### !end-answer

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: 37d59847-dc43-44d8-b5df-89c2dbeb9c4e
* title: Insert Complexity

##### !question

Get out a pencil and paper, and analyze the runtime complexity of inserting a record into a max-heap.

What is the algorithm doing at each step? How many steps does it take in the worst case? What _is_ the worst case?

What parallels can you draw to similar work with other data structures?

If the heap has a capacity of \\(c\\) and currently contains \\(n\\) records, the time complexity of inserting a new record is...

##### !end-question

##### !options

* \\(O(1)\\)
* \\(O(log(n))\\)
* \\(O(log(c))\\)
* \\(O(n)\\)
* \\(O(c)\\)

##### !end-options

##### !answer

* \\(O(log(n))\\)

##### !end-answer

##### !hint

The worst case is when the newly inserted record has higher priority than anything currently in the heap.

In this case, insert walks up the path from a leaf all the way to the root, so that if \\(h\\) is the height of the tree insert will perform \\(h\\) swaps.

Since a heap is a perfectly balanced tree, we know that the height is \\(O(log(n))\\).

##### !end-hint

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: 20e47915-800f-407e-b21b-e5004be5ff6b
* title: Remove-Max Strategy

##### !question

Which of the following describes the strategy for removing the highest-priority record from a max-heap?

##### !end-question

##### !options

* Use linear search to find the record with the highest priority
* Use binary search to find the record with the highest priority
* The highest-priority record is at the end of the array, so you can just remove it
* The highest-priority record is at the root. Swap this with the last record, then "sink" the new root down to the right place by repeatedly swapping with its larger child.

##### !end-options

##### !answer

* The highest-priority record is at the root. Swap this with the last record, then "sink" the new root down to the right place by repeatedly swapping with its larger child.

##### !end-answer

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
<!-- >>>>>>>>>>>>>>>>>>>>>> BEGIN CHALLENGE >>>>>>>>>>>>>>>>>>>>>> -->
<!-- Replace everything in square brackets [] and remove brackets  -->

### !challenge

* type: multiple-choice
* id: b10ea7de-4464-40c6-9b2c-f0c812d75e6a
* title: Remove-Max Complexity

##### !question

Get out a pencil and paper, and analyze the runtime complexity of removing the highest-priority record from a max-heap.

What is the algorithm doing at each step? How many steps does it take in the worst case? What _is_ the worst case?

What parallels can you draw to similar work with other data structures?

If the heap has a capacity of \\(c\\) and currently contains \\(n\\) records, the time complexity of inserting a new record is...

##### !end-question

##### !options

* \\(O(1)\\)
* \\(O(log(n))\\)
* \\(O(log(c))\\)
* \\(O(n)\\)
* \\(O(c)\\)

##### !end-options

##### !answer

* \\(O(log(n))\\)

##### !end-answer

##### !hint

The worst case is when the record that gets swapped with the root will need to sink all the way back down to the lowest level of the heap, for example if it's the lowest priority record.

In this case remove acts much like insert in reverse. It walks down a path of length \\(h = O(log(n))\\) from the root to the new leaf position, swapping each time.

##### !end-hint

### !end-challenge

<!-- ======================= END CHALLENGE ======================= -->
