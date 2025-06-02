# EX 5A Minimum Cost Path
## DATE:
## AIM:
To write a Python program using A Naive recursive implementation of Minimum Cost Path Problem.




## Algorithm
1. If either m or n is out of bounds (<0), return a large value (infinity).
2. If m and n are both 0, return the starting cell cost[0][0].
3. Recursively calculate the minimum cost from three directions: diagonal (m-1,n-1), up (m-1,n), and left (m,n-1).
4. Add the current cell cost[m][n] to the minimum of the three recursive calls.
5. Return the total minimum cost to reach cell (m,n) from (0,0).   

## Program:
```
/*
A program to implement to find the Minimum Cost Path Problem using a  Naive recursive Approach.

Developed by: 
Register Number:
R = int(input())
C = int(input())
import sys
def minCost(cost, m, n):
    if(n<0 or m<0):
        return sys.maxsize
    elif(m==0 and n==0):
        return cost[m][n]
    else:
        return cost[m][n]+min(minCost(cost,m-1,n-1),minCost(cost,m-1,n),minCost(cost,m,n-1))
def min(x, y, z):
    if (x < y):
        return x if (x < z) else z
    else:
        return y if (y < z) else z
cost= [ [1, 2, 3],
        [4, 8, 2],
        [1, 5, 3] ]
print(minCost(cost, R-1, C-1))
*/
```

## Output:

![image](https://github.com/user-attachments/assets/3b754f51-c435-4b66-89b4-7669ee9e77e3)


## Result:
Thus the above program was executed successfully for finding the minimum cost.
