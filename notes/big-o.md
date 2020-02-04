Carefully concider each step of an algorithm and it's properties. Defining both how long something would take depending on an input and how it is independent of related to other parts of the algorithm is key in being able to CORRECTLY simplify down a big O expression. There are algorithms that depend on multiple inputs where each can  effect the big O individually, or possibly interacting to become thier own variable in the big O expression.

Review page 52

Analyze the math used in the algorithm, not just the form of for loops and amount of recursive calls for the algorithm. Search for pieces of math that affect the bounds of the calls, which then effect the bounds of the big O. For example, looping through something where the conditional has math that relates to the index being used, or the incrementation section has math. Incrementation is constant, this means the conditional isn't necessarily linear with the loop, so it's exciting wouldn't be done in a different big O time. Same thing with the incrementation, as this section determines how the state of the for loop changes, so if the index shifts by multiplication, then it's possible the ending conditional is reached in a Log time, for example.

- For the mathematical checking of dynamic bound changes, addition and subtraction will probably cause linear effects, and multiplication and division will cause logotithmic and exponential effects.
- multiplication by self causes polynomial bounding changes, division causes exponential/logarithmic bounding changes.

-N
-N
-1
-N, b is constant while sum changes linearly with addition

You got them wrong. You didnt pay attention to the fact that the upper bound a isn't constant, it changes depending on the input

-LogN, the bounds for returning are min and Max. At each call, one of the other gets changed to be halfway between each other. This means the search size decreases by half every iteration across the linearly bounded space.
 -Sqrt(n), the lower bound increases quadratically, so that means it approaches the upper bound at that rate. This means the lower bound would appoarch the upper bound at the same rate is the upper bound was rooted. The rate of increase of the quadratic argument is linear due to addition, so that doesn't have any multiplicative effect on the for loop.
 -N, if it is not balanced, the worst case structure of a binary search tree is everything being to one side, so all elements must be traversed causing and n-time traversal
 -N, if the binary tree does not have a heuristic, then there are no assumptions that can be made, so an traversal of all nodes must be attempted in order to make sure that the value being searched for is reached
 -n^2, for loop bounds increase linearly in foreaxh, and work done inside addtoarray is linear as well
 -log10N, the bound N, passed in, approaches the bottom bound by division, causing it to decrease its size by a base factor Everytime.

Practice checking whether or not bounds are variables or not, allowing them to increase as they are changed. Be attentive about bounds that are sent into the function, that undeniably a source of complexity that definitively indicates big O factor.