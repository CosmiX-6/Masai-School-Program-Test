# APPLY BASIC MATHS

Given, an array A (index starting from 0) with N elements. You CAN remove only that element which makes the sum of ALL the remaining elements exactly divisible by 7.
Your task is to find the first array index of the smallest element that can be removed.
Input Format
The first line contains a single integer N.
Next line contains N space separated integers A[k] , 0 < k < N - 0 based indexing
_________________________________________________________________________________
Constraints
1 < N < 100000
0 < A[k] < 1000000000
_________________________________________________________________________________
Output Format
---------------------------------------------------------------------------------
Print a single line containing one integer, the first array index of the smallest element that CAN be removed, and -1 if there is no such element that he can remove!
_________________________________________________________________________________
Sample Input 0
---------------------------------------------------------------------------------
5
14 7 8 2 4
_________________________________________________________________________________
Sample Output 0
---------------------------------------------------------------------------------
1
_________________________________________________________________________________
Explanation 0
---------------------------------------------------------------------------------
Both 14 and 7 are valid answers, but since 7 is the smallest, the required array index is 1.
_________________________________________________________________________________
Python Code:
=================================================================================
```n=int(input())
A=list(map(int,input().strip().split()))
temp=sorted(A)
for i in range(len(A)):
    temp[i]=0
    s=sum(temp)
    temp=sorted(A)
    if s%7==0:
        flag=True
        break
    else:
        flag=False
if flag==True:
    print(A.index(temp[i]))
else:
    print(-1)
```
