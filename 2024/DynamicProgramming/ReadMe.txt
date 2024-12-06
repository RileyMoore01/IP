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
          ```
          // Pseudocode example for bottom-up
          
          F = array of length (n + 1)
          F[0] = 0
          F[1] = 1
          for i from 2 to n:
              F[i] = F[i - 1] + F[i - 2]
          ```
  2.) Top-down, also known as memoization
          - Top-down is implemented with recursion and made efficient with memoization.
          - memoizing a result means to store the result of a function call, usually in a hashmap or an array, so that when the same function call is made again, we can simply return the memoized result instead of recalculating the result.
          ```
          // Pseudocode example for top-down
          
          memo = hashmap
          Function F(integer i):
              if i is 0 or 1: 
                  return i
              if i doesn't exist in memo:
                  memo[i] = F(i - 1) + F(i - 2)
              return memo[i]
          ```

A bottom-up implementation's runtime is usually faster, as iteration does not have the overhead that recursion does.
A top-down implementation is usually much easier to write. This is because with recursion, the ordering of subproblems does not matter, whereas with tabulation, we need to go through a logical ordering of solving subproblems.



Strategic Approach  -------------------------------------------------------------------------------------------


Common Patterns  -----------------------------------------------------------------------------------------------


Dynamic Programming for Paths in a Matrix  ---------------------------------------------------------------------
