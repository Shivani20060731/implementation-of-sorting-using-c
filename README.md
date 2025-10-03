# implementation-of-sorting-using-c
Implementation of Sorting in C++

Aim

To explore and implement various sorting algorithms in C++ using both array indexing and pointer manipulation.

Software Used

Online C++ Compiler


Theory of Sorting

Sorting is the process of arranging data in a particular order, typically ascending or descending. It plays a crucial role in searching, database management, and optimization problems. Sorting algorithms differ in their time complexity, space usage, stability, and implementation simplicity.

Why Sorting is Important?

Makes searching faster (e.g., Binary Search requires sorted data).

Improves efficiency in data storage and retrieval.

Is a foundation for more advanced algorithms (like merge sort, quicksort, heap sort).


In this experiment, we implement and compare:

1. Bubble Sort using pointers


2. Insertion Sort


3. Bubble Sort using arrays

Program 1: Bubble Sort using Pointers

Explanation of Code

Bubble Sort repeatedly compares adjacent elements and swaps them if they are in the wrong order.

In this implementation, pointers are used instead of array indices.

Pointer arithmetic (ptr and ptr+1) allows direct memory access and manipulation.

The algorithm makes multiple passes, and after each pass, the largest unsorted element moves to its correct position at the end.

Sorting is in-place (no extra memory needed).


Complexity

Time Complexity: O(n²) average and worst case.

Space Complexity: O(1).

Stability: Stable (does not change relative order of equal elements).


Algorithm

1. Start.


2. Input array elements.


3. Repeat for (n - 1) passes:

Set pointer ptr to the first element.

Compare *ptr with *(ptr+1).

If *ptr > *(ptr+1), swap them.

Increment pointer and continue until unsorted portion ends.



4. After each pass, reduce the comparison range by one.


5. Repeat until all elements are sorted.


6. Print sorted array.


7. Stop.

Program 2: Insertion Sort

Explanation of Code

Insertion Sort works by building a sorted portion of the array one element at a time.

The first element is assumed to be sorted.

Each subsequent element (key) is compared with elements in the sorted portion.

Larger elements are shifted one position to the right until the correct position for the key is found.

The key is then inserted.


Complexity

Time Complexity:

Best case (already sorted): O(n).

Average/Worst case: O(n²).


Space Complexity: O(1).

Stability: Stable.


Algorithm

1. Start.


2. Input array elements.


3. Assume first element is sorted.


4. For each unsorted element:

Store it as the key.

Compare it with elements in the sorted portion.

Shift larger elements one position right.

Insert the key at its correct position.



5. Repeat until all elements are placed correctly.


6. Print sorted array.


7. Stop.

Program 3: Bubble Sort (Array-based)

Explanation of Code

Similar to pointer-based Bubble Sort but uses array indices.

Outer loop counts number of passes.

Inner loop compares adjacent array elements and swaps if needed.

After each pass, the largest unsorted element is placed at the correct position at the end.


Complexity

Time Complexity: O(n²) in average and worst case.

Space Complexity: O(1).

Stability: Stable.


Algorithm

1. Start.


2. Input array elements.


3. Repeat for (n - 1) passes:

For each pass, compare arr[i] with arr[i+1].

Swap if arr[i] > arr[i+1].

Continue until end of unsorted portion.



4. Increment pass counter and repeat until sorted.


5. Print sorted array.


6. Stop.


Conclusion

The three sorting implementations—Pointer-based Bubble Sort, Insertion Sort, and Array-based Bubble Sort—highlight the core principles of elementary sorting algorithms.
