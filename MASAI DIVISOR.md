# MASAI DIVISOR

You are provided 3 integers: left, right and k. Your task is to write a program that finds out count of all such numbers between left and right (both inclusive) which are divided by k.
Input Format
First line contains 3 space separated integers which are left, right and k respectively.
_________________________________________________________________________________
Constraints
---------------------------------------------------------------------------------
l,r,k<10000
_________________________________________________________________________________
Output Format
---------------------------------------------------------------------------------
Output the count of such numbers
_________________________________________________________________________________
Sample Input 0
---------------------------------------------------------------------------------
1 10 1
_________________________________________________________________________________
Sample Output 0
---------------------------------------------------------------------------------
10

_________________________________________________________________________________
Python Code:
=================================================================================
```left,right,k=map(int,input().strip().split())
count=0
for i in range(left,right+1):
    if i%k==0:
        count+=1
print(count)
```
