Minimum ASCII Delete Sum for Two Strings 

1.Define the problem/solution recursively 

my main goal is to find the lowest ASCII sum of deleted characters to make the 2 inputs the same. 
In order to solve this, i will need to solve a smaller problem: to find some 
kind of data base to store sum of the other string.

//dp[i][s2.length()] = dp[i+1][s2.length()] + s1.codePointAt(i);
//dp[i][j] = dp[i+1][j+1];
//dp[i][j] = Math.min(dp[i+1][j] + s1.codePointAt(i),
//                    dp[i][j+1] + s2.codePointAt(j));

2.Briefly talk about how you plan to store solutions to sub-problems and combining them to solve the global problem

for this problem i plan on using 2d int array. The array will hold the sum of the other string cumulatively. if 
the strings at the same position contain the same char, we will ignore those characters. If they are different, we
will remove at least one of then, and in the end we'll return dp[0][0]
