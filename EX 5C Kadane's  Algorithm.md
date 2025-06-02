# EX 5C Kadane's Algorithm
## DATE:
## AIM:
To write a python program to find the maximum contiguous subarray.


## Algorithm
1. Initialize max_so_far and curr_max with the first element of the array.
2. Traverse the array from index 1 to end.
3. At each step, update curr_max = max(current element, curr_max + current element).
4. Update max_so_far = max(max_so_far, curr_max) to store the maximum sum so far.
5. Return max_so_far as the maximum contiguous subarray sum.
## Program:
```
/*
To implement the program to find the maximum contiguous subarray.


Developed by: D Vergin Jenifer
Register Number: 212223240174
def maxSubArraySum(a,size):
    max_so_far=a[0]
    curr_max=a[0]
    for i in range(1,size):
        curr_max=max(a[i],curr_max+a[i])
        max_so_far=max(max_so_far,curr_max)
    return max_so_far
    
n=int(input())  
a =[] #[-2, -3, 4, -1, -2, 1, 5, -3]
for i in range(n):
    a.append(int(input()))
  
print("Maximum contiguous sum is", maxSubArraySum(a,n))
*/
```

## Output:

![image](https://github.com/user-attachments/assets/3fb0ddc9-b5dd-4f3d-9bba-2eb006f16b36)


## Result:
Thus the program was executed successfully for finding the maximum contiguous sum of subarray..
