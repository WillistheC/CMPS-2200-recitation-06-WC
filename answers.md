# CMPS 2200 Recitation 06
## Answers

**Name:**_________________________
**Name:**_________________________


Place all written answers from `recitation-06.md` here for easier grading.



- **1)** Before we implement a heap, let's consider if we just maintain
 an unordered list/sequence. 

  - **1a) (1 pt)** What is the work/span of *deleteMin*?
 
  Before implementing a heap, *deleteMin* would be done by comparing pairs of elements in parallel, finding the min in combination, and deleting the final value.

  Work: This gives $W(n) = 2W(\frac{n}{2}) + 1 = O(n)$

  Span: The longest chain of dependency would be the height of the tree, so when $\frac{n}{2^{h}} = 2$, so $S(n) = O(logn)$

  - **1b) (1 pt)** What is the work/span ofand *insert(x)*?
 
  Before implementing a heap, *insert(x)* is just an append command; $W(n) = O(1), S(n) = O(n)$

- **2a) (1 pt)** For a heap with $n$ elements, what does this imply about the depth of the associated almost-complete binary tree?

The heap will have binary splits until $\frac{n}{2^h} = 1$ where $h$ is the depth, so the depth is equal to $log{_2}{n}$ rounded down to the nearest whole number (a one element heap counts as depth zero)

- **2b) (1 pt)** By maintaining the heap property, where is the minimum element of
  the heap? Can we say anything about the maximum element?

The minimum element will be the root of the heap, and the maximum will be a the bottom level / maximum depth

- **4a) (1 pt)** What is the work/span of *reheapUp*($x$)?

- **4b) (1 pt)** What is the work/span of *reheapDown*($x$)? 

- **6) (1 pt)** What is the work and span of `heapsort`?
