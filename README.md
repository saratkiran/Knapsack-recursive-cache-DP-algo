# Knapsack-recursive-cache-DP-algo
Compare knapsack algorithms with timings analysis
Sarat Kiran Andhavarapu

Written in Java.
Uncomment the code between the horizontal dotted lines for corresponding solutions in Java file.
Cap variable gives the capacity of the kanpsack 
Change the no_objects variable to change the number of input objects 
All three solutions are written in seperate functions. To execute each uncomment the correponding section.

Folders - 
  1. Raw Data - Inputs used for testing all the algorithms 
  2. Java Code - Code used for the algos 
  3. Graphs - Graphs with different parameters to measure the efficiency of the algorithm
  4. Report - Detailed information about graphs and  observations.


Given: n items each of size s[i] and value v[i] and maximum capacity S. All objects have a non-zero size and a positive value
Find a subset of objects that fit into the knapsack. It is not necessary that they exactly fit into the knapsack
Such that the sum of the values of the objects put in the knapsack is maximized.

1) A recursive solution to the above Knapsack optimization problem.

3) A caching (memorizing) solution to this problem. 

4) A dynamic programming solution to this problem

Empirical Studies: 

For randomized data, a graph that measures the average cpu time of the recursive solution as a function of n.
Pick a fixed S as 1000 and assign the sizes of the objects from 1 to 1000 using a uniform random distribution. 
Start at n=6 and go as large as you can within reasonable running times, increasing the problem size by 1 each time. 
Produce a semi-log graph where n is the size of the problem (number of objects) along the x axis and y is the average run time (log scale). 
If your code is running correctly your graph should illustrate a near-straight line. Compute the slope of the line and explain the value you obtained.

Here you will compare the run-time performance of the dynamic programming solution with the caching solution under different random data distributions and much larger problem sizes. 
Given n is the problem size and m is the capacity of the knapsack for each experiment set m= 10*n. In each experiment, generate the sizes of the n objects need from a uniform random distribution between min-size and m/10. 
You will run the experiments under two different distributions (a) wide where min-size is 1, and narrow where min-size is m/20. Start at size 64 and go as large as you can within reasonable running times, increasing the problem size by a factor of 2 each time. 
Produce a log-log graph where x is the log of the size of the problem and y is the log of the average running time. The graph should have two lines, one for wide and one for narrow.
