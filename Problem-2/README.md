Partition to K Equal Sum Subsets

1.Define the problem/solution recursively 

my main goal is to find whether it's possible to divide the given array into k non-empty subsets whose sums are all equal. In order to solve this, i will need to solve a smaller problem: to find some kind of data base to store both if my current position at the array can use this number as a subset, and another to check the total of the numbers that were accepted.

//dp[future] = true;
//total[future] = total[state] + nums[i];

2.Briefly talk about how you plan to store solutions to sub-problems and combining them to solve the global problem

for this problem i plan on using an array of booleans and another int array to keep track of the total. after that, the array boolean array will be filled with true or false values depending if we can use the current number. if we can then we will store that number in our other int array. afterwards i will return the last element of the boolean array.
