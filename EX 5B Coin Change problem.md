# EX 5B Coin Change Problem
## DATE:
## AIM:
To compute the fewest number of coins that we need to make up the amount given.


## Algorithm:
1. Initialize a dp array of size (amount + 1) with a large value (amount + 1), and set dp[0] = 0.
2. For each amount i from 1 to amount, check all coins.
3. If coin <= i, update dp[i] = min(dp[i], dp[i - coin] + 1).
4. Repeat until dp[amount] holds the minimum number of coins needed to make the amount.
5. Return dp[amount] if it's updated; otherwise, return -1 (not possible).  

## Program:
```
/*
Create a python function to compute the fewest number of coins that we need to make up the amount given.

.
Developed by: D Vergin Jenifer 
Register Number: 212223240174
class Solution(object):
    def coinChange(self, coins, amount):
        dp=[amount+1]*(amount+1)
        dp[0]=0
        for i in range(1,amount+1):
            for coin in coins:
                if coin<=i:
                    dp[i]=min(dp[i],dp[i-coin]+1)
        return dp[amount] if dp[amount]!=amount+1 else -1
       
      
      
ob1 = Solution()
n=int(input())
s=[]
amt=int(input())
for i in range(n):
    s.append(int(input()))


print(ob1.coinChange(s,amt))
*/
```

## Output:

![image](https://github.com/user-attachments/assets/028c48c7-4e30-4faa-a86e-a1193a963e9d)


## Result:
Thus the program was executed successfully for finding the minimum number of coins required to make amount.
