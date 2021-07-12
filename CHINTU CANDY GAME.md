# CHINTU CANDY GAME

Chintu wants to play a game .
The game has following rules:
Chintu will be given S points.he has to choose some positive integer number 1=x=s
Chintu can perform the following operation any number of times (possibly, zero): buy some candies that costs exactly x points and obtain [x/10] points as a cashback (in other words, Chintu spends x points and obtains ?x/10? back). The operation ?a/b? means a divided by b rounded down.
It is guaranteed that he can always buy some candies that costs x for any possible value of x.
Your task is to say the maximum number of points Chintu can spend if he buys candies optimally so that he can win the game.
Input Format
The first line of the input contains one integer t indicates number of testcases.
The next t lines describe test cases. Each test case is given on a separate line and consists of one integer s — the number of Points Chintu initially has.
_________________________________________________________________________________
Constraints
---------------------------------------------------------------------------------
1 = s = 10^9
1 = t = 10^4
_________________________________________________________________________________
Output Format
---------------------------------------------------------------------------------
For each test case print the answer on it the maximum number of Points Chintu can spend if he buys candies optimally.
_________________________________________________________________________________
Sample Input 0
---------------------------------------------------------------------------------
6
1
10
19
9876
12345
1000000000
_________________________________________________________________________________
Sample Output 0
---------------------------------------------------------------------------------
1
11
21
10973
13716
1111111111
_________________________________________________________________________________
Explanation 0
---------------------------------------------------------------------------------
For example, if Chintu has s=19 Points then the maximum number of Points he can spend is 21. Firstly, he can spend x=10 Points, obtain 1 Point as a cashback. Now he has s=10 Points, so can spend x=10 Points, obtain 1 Point as a cashback and spend it too.

_________________________________________________________________________________
Python Code:
=================================================================================
```li=[int(input()) for i in range(int(input()))]
for i in li:
    spend=0
    while i>9:
        q=i//10
        i=(i%10)+q
        spend=spend+(q*10)
    print(spend+i)

```
