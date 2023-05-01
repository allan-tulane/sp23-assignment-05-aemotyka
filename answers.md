# CMPS 2200 Assignment 5
## Answers

# **Name:**_Alex Motyka_


# Place all written answers from `assignment-05.md` here for easier grading.





# - **1a.**
# A greedy algorithm to turn an N dollars into as few coins as possible would be to find the highest power of two that is less N, include the coin with that value, subtract that value from N, and recurse/repeat. This approach results in the smallest possible number of coins and is optimal because every coin is a power of two.

# - **1b.**
# Work = O(log n) because each recursion divides input N by 2.
# Span = O(log n) as well because this algorithm cannot be parallelized.

# - **2a.**
# A counterexample: breaking $8 into coins with values $6, $4, $1. By the greedy algorithm from 1a, $6 would be chosen first, followed by $1 and then $1 again. However, this results in 3 coins, while two $4 coins would be fewer coins and also add up to $8. Consistantly choosing the highest valued coin and then recursing is not optimal in this case because there is no longer a coherent pattern among the available coins.

# - **2b.**
# My program would create a binary tree with input value N at the root. Each node would represent one of the two highest valued coins less that or equal to the value in the previous node subtracted from the previous node, and this pattern would repeat until every leaf node = 0. The shortest path to a leaf node in this tree would then give the optimal solution and combination of coins. This problem would also require a dictionary with each path and operation in the tree to prevent redundant recomputations.
# Work = Span = O(log n)

# - **3a.**
# (In main.py)

# - **3b.**
# (In main.py)

# - **3c.**
# (In main.py)
