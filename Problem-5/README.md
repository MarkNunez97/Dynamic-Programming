countSubstrings

1.Define the problem/solution recursively 

my main goal is to find how many palindromic substrings are in the string. In order to solve this, 
i will need to solve a smaller problem: to find some kind of data base to store if at my current pointers,
the characters are the same.


2.Briefly talk about how you plan to store solutions to sub-problems and combining them to solve the global problem

for this problem i plan on using an 2d boolean array. The array will be filled with true or false
depending if the the characters are the same at the current pointers. we would then increase our result
only if our 2d array is true.after going through the string, simply return the counter.
