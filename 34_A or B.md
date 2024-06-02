# A or B

There are two problems in a contest.

    Problem A is worth 500500 points at the start of the contest.
    Problem B is worth 10001000 points at the start of the contest.

Once the contest starts, after each minute:

    Maximum points of Problem A reduce by 22 points .
    Maximum points of Problem B reduce by 44 points.

It is known that Chef requires XX minutes to solve Problem A correctly and YY minutes to solve Problem B correctly.

Find the maximum number of points Chef can score if he optimally decides the order of attempting both the problems.
Input Format

    First line will contain TT, number of test cases. Then the test cases follow.
    Each test case contains of a single line of input, two integers XX and YY - the time required to solve problems AA and BB in minutes respectively.

```java
import java.util.*;
import java.lang.*;
import java.io.*;

class Codechef
{
	public static void main (String[] args) throws java.lang.Exception
	{
        Scanner in=new Scanner(System.in);
        int t=in.nextInt();
        while(t-->0)
        {
            int x=in.nextInt();
            int y=in.nextInt();
            
            int result1=(500-(x*2))+(1000-((x+y)*4));
            int result2=(1000-(y*4))+(500-((x+y)*2));
            if(result1>=result2)
                System.out.println(result1);
            else
                System.out.println(result2);
        }

	}
}
```
