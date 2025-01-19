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

:stacks:
- last in first out(LIFO).
- push() to put or add a value at the end of the stack
- pop() to remove the value at the end of the stack
- peek() to check the value at the end of the stack
- length() or size() to check the length or size of the stack

:sets:
- set data structure is like an array except there are no duplicate items.
- values are not in any particular order.
- typical use is to check for the presence of an item.
