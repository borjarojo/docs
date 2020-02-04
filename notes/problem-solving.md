Optomization:
If there are comparisons to be made, and a set of possibilities for the things to compare, find ways to be able to only do comparisons on the smallest set of stuff needed. 

For example, comparing the permutations of a smaller string to see if they are contained in a larger string:

The brute force way of doing this is to go generate all the permutations and see if any of them are in each of the possible section of the larger string. There are many comparisons being made that would most likely be redundant when done raw like this. The reason is because there are indeed many permutations of the smaller string that are not the one being checked for. In fact, the permutation being checked for is possibly only one of the possibilities, so checking through all the permutations generated from the smaller string is very expensive.

A way to optimize is to reverse the comparison and see if the permutation available from the larger string is one in the smaller string. If it is cheaper to check to see if the section of the larger string is a permutation the smaller string without calculating all of the permutations of the smaller string, then this would yield a faster result.

The take away to notice here is that he brute force method tends to consider all possibilities. It is usually a method that applies to a larger more general set of problems. The way to optimize algoirthmically is to pay attention to what information is actually present in a specific instance, and to only generalize on those things that vary within the problem.

Instead generating all the possible permutations for all possibilities, check to see if the current section is a permutation. Attack the problem by identifying what is actually there, manifested in the information given in context, and deal only with those things.