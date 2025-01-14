:big_O_notation: "How code slows as data grows." 
1. Describes the performance of an algorithm as the amount of data increases.
2. Machine independent (# of steps to completion)
3. Ignore smaller operations O(n + 1) -> 0(n)

example:  O(1) - constant time
          O(n) - linear time
          O(log n)
          O(n^2)

n = amount of data (it's a variable like x)

O(1) - constant time
* random access of an element in an array
* inserting at the beginning of linkedlist

O(log n) - logarithmic time
* binary search

O(n) - linear time
* looping through elements in an array
* searching through a linkedlist

O(n log n) - quasilinear time
* quicksort
* mergesort
* heapsort

O(n^2) - quadratic time
* insertion sort
* selection sort
* bubblesort

O(n!) - factorial time
* traveling salesman problem

