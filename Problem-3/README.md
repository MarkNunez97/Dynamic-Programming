Integer Break

1.Define the problem/solution recursively 

my main goal is to find at least 2 positive integers and maximize the product of those integers. 
In order to solve this, i will need to solve a smaller problem: to find some kind of data base to 
store what the biggest int can be generated from the integers that make up the number provided.

//dp[i] = Math.max(dp[i],Math.max(j, dp[j]) * Math.max(i - j, dp[i - j]));

2.Briefly talk about how you plan to store solutions to sub-problems and combining them to solve the global problem

for this problem i plan on using an int array. The array will be filled with the maximum product at the
current position of 2 pointers. after going through all of the numbers, simply return the array at position 'n'.
