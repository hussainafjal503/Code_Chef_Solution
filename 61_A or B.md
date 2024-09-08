# A or B

There are two problems in a contest.

Problem A is worth 500500 points at the start of the contest.
Problem B is worth 10001000 points at the start of the contest.

Once the contest starts, after each minute:

Maximum points of Problem A reduce by 22 points .
Maximum points of Problem B reduce by 44 points.

It is known that Chef requires XX minutes to solve Problem A correctly and YY minutes to solve Problem B correctly.

Find the maximum number of points Chef can score if he optimally decides the order of attempting both the problems. Input Format

First line will contain TT, number of test cases. Then the test cases follow.
Each test case contains of a single line of input, two integers XX and YY - the time required to solve problems AA and BB in minutes respectively.

# Java
```java
/* package codechef; // don't place package name! */

import java.util.*;
import java.lang.*;
import java.io.*;

/* Name of the class has to be "Main" only if the class is public. */
class Codechef
{
	public static void main (String[] args) throws java.lang.Exception
	{
		// your code goes here
		Scanner s = new Scanner(System.in);
		int t = s.nextInt();
		while(t-->0)
		{
		    int a = s.nextInt();
		    int b = s.nextInt();
		    int c = 500-(a*2); 
		    int d =1000-(a+b)*4;
		    int e = 1000-(b*4); 
		    int f = 500-(a+b)*2;
		    if((c+d)>(e+f))
                System.out.println(c+d);
            else
                System.out.println(e+f);
		}
	}
}
```
