LeetCode's Dynamic Programming Prep
Here are my notes divided into the courses sections.


Intro  --------------------------------------------------------------------------------------------------------
Things to note when thinking about using DP
  1.) The problem can be broken down into "overlapping subproblems"
  2.) The problem has an "optimal substructure" - soultions for the overlapping subproblems

Greedy Problems - optimal substrucutre, but not overlapping subproblems
Divide & Conquer Algorithms - break a problem into subproblems, but these subproblems are not overlapping (which is why DP and divide and conquer are commonly mistaken for one another)

There are 2 ways to implement a DP algorithm. 
  1.) Bottom-up, also known as tabulation
          - Bottom-up is implemented with iteration and starts at the base cases
  2.) Top-down, also known as memoization
          - Top-down is implemented with recursion and made efficient with memoization.
          - memoizing a result means to store the result of a function call, usually in a hashmap or an array, so that when the same function call is made again, we can simply return the memoized result instead of recalculating the result.



Strategic Approach  -------------------------------------------------------------------------------------------


Common Patterns  -----------------------------------------------------------------------------------------------


Dynamic Programming for Paths in a Matrix  ---------------------------------------------------------------------
