Maximum length of pair chain

1.Define the problem/solution recursively 

my main goal is to find the longest pair that can be formed. In order to solve this,
i will need to solve a smaller problem:to find some kind of data base to store what 
the length of the chain is while traversing it.

2.Briefly talk about how you plan to store solutions to sub-problems and combining them to solve the global problem

for this problem i plan on using an int array. The array will be filled with the max length of the chain
while we are traversing it. we only increase our length after we check if the next pos is less than the
previous one. after going through all of the array, we go through our array again and find that largest
length.
