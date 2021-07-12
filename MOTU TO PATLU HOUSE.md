# MOTU TO PATLU HOUSE

Motu decided to visit his friend Potlu. It turned out that the Motu's house is located at point 0 and his friend's house is located at point x (x > 0) of the coordinate line. In one step the Motu can move 1, 2, 3, 4 or 5 positions forward. Determine, what is the minimum number of steps he need to make in order to get to his friend's house.
Input Format
First and the only line contain the integer n which denotes the position of his friend's house.
_________________________________________________________________________________
Constraints
---------------------------------------------------------------------------------
1 <= n <= 10^6
_________________________________________________________________________________
Output Format
---------------------------------------------------------------------------------
Output contains a single line denoting the minimum number of steps.
_________________________________________________________________________________
Sample Input 0
---------------------------------------------------------------------------------
26
_________________________________________________________________________________
Sample Output 0
---------------------------------------------------------------------------------
6
_________________________________________________________________________________
Explanation 0
---------------------------------------------------------------------------------
For n = 26, Motu can move as
5 --> 5 --> 5 --> 5 --> 5 --> 1
Hence he needed 6 steps to reach at position 26.

_________________________________________________________________________________
Python Code:
=================================================================================
```n=int(input())
sum=0
for i in range(5,0,-1):
    if n>0:
        sum=sum+(n//i)
        n=n%i
    else:
        break
print(sum)
```
