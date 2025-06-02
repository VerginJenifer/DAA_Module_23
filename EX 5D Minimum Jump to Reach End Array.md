# EX 5D Minimum Jump to Reach End Array
## DATE:
## AIM:
To write a python program for finding the minimum number of jumps needed to reach end of the array using Dynamic Programming.


## Algorithm
1. Initialize a jumps[] array to store the minimum jumps needed to reach each index.
2. Set jumps[0] = 0; if the array is empty or arr[0] == 0, return infinity (not reachable).
3. For each index i from 1 to n-1, set jumps[i] to infinity.
4. For each j from 0 to i-1, if i is reachable from j and jumps[j] is valid, update jumps[i] = min(jumps[i], jumps[j] + 1).
5. Return jumps[n-1], the minimum jumps to reach the end.  

## Program:
```
/*
To implement the program to finding the minimum number of jumps needed to reach end of the array.


Developed by: D Vergin Jenifer
Register Number: 212223240174
def minJumps(arr, n):
    jumps=[0 for i in range(n)]
    if(n==0) or (arr[0]==0):
        return float('inf')
    jumps[0]=0
    for i in range(1,n):
        jumps[i]=float('inf')
        for j in range(i):
            if(i<=j+arr[j]) and (jumps[j]!=float('inf')):
                jumps[i]=min(jumps[i],jumps[j]+1)
    return jumps[n-1]
arr = []
n = int(input()) #len(arr)
for i in range(n):
    arr.append(int(input()))
print('Minimum number of jumps to reach','end is', minJumps(arr,n))
 
*/
```

## Output:

![image](https://github.com/user-attachments/assets/42040b11-448a-4c9d-bd09-8e47425b3a5c)


## Result:
Thus the program was executed successfully for finding the minimum number of jumps to reach end.
