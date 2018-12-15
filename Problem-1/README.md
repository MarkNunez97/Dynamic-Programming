# Dynamic-Programmingperfect square

1.Define the problem/solution recursively 

my main goal is to find the least # of perfect square numbers that will add up to n. In order to solve this, i will need to solve a smaller problem: to find some kind of data base to store the amount of perfect squares needed to solve the current number until I reach n.

//dp[i] = min;

2.Briefly talk about how you plan to store solutions to sub-problems and combining them
to solve the global problem

for this problem i plan on using an array the size of n+1. it is n+1 because the first element will always be 0. after that, the array is going to be filled with values of least perfect squares it takes to build that number. for ex. if we do numSquares(4), the array should look as follows dp = {0,1,2,3,1} because:

	least # of perfect squares for 0 = 0;
	least # of perfect squares for 1 = 1;
	least # of perfect squares for 2 = 2; (square root of 1 twice)
	least # of perfect squares for 3 = 3; (square root of 1 3 times)
	least # of perfect squares for 4 = 1; (square root of 4 once)

i would then return the last element.
