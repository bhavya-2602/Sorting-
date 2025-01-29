Argue Correctness of Selection Sort

Loop invariant method is used to prove correctness of selection sort.In this method it shows certain conditions holds before and after each iteration of algorithm.

Selection Sort Algorithm Recap- Works by selecting the smallest element from the unsorted portion of array and swapping with first unsorted element.The process continues until the entire array is sorted.
Loop Invariant Statement
In beginning of each iteration 
i
i of the outer loop, the subarray arr[0] to arr[i-1] contains the smallest 
𝑖
i elements in sorted order.

Step 1: Initialization (Base Case)
Before the first iteration (
𝑖
=
0
i=0), the sorted portion of the array is empty.
This trivially establishes the loop invariant, since an empty subarray is always sorted.

Step 2: Keep it up (Inductive Step)

During each iteration:

The goal of the algorithm is, it finds the minimum element from the unsorted part of the array(arr[i] - arr[n-1]).

It replaces this smallest element with arr[i]. Thus the subarray arr[0] to arr[i] will be sorted and will have the minimum
𝑖
+
1
i+1 elements in the correct order.
By induction, if the invariant holds at the start of iteration 
𝑖
i, it will hold for iteration 
𝑖
+
1
i+1 as well.
Step 3: Termination
At the end of the last iteration (
𝑖
=
𝑛
−
1
i=n−1), the entire array is sorted because:
the sorted portion extends to the whole array.

Time Complexity Analysis
Best Case: 
𝑂
(
𝑛
2
)
O(n 
2
 )
Worst Case: 
𝑂
(
𝑛
2
)
O(n 
2
 )
Average Case: 
𝑂
(
𝑛
2
)
O(n 
2
 )
Even in the best case (already sorted array), Selection Sort still performs 
𝑂
(
𝑛
2
)
O(n 
2
 ) 

 Conclusion
 Selection sort is correct because it takes responsibility that the sorted portion of the array grows correctly.
 It is not applicable to large arrays beacuse,
 𝑂
(
𝑛
2
)
O(n 
2
 ) complexity.
It is beneficial to small datasets.
 
 
