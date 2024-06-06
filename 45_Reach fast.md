# Reach fast

Chef is standing at coordinate AA while Chefina is standing at coordinate BB.

In one step, Chef can increase or decrease his coordinate by at most KK.

Determine the minimum number of steps required by Chef to reach Chefina.

Input Format

   The first line of input will contain a single integer TT, denoting the number of test cases.
  Each test case consists of three integers X,Y,X,Y, and KK, the initial coordinate of Chef, the initial coordinate of Chefina and the maximum number of coordinates Chef can move in one step.
```java
import java.util.*;
import java.lang.*;
import java.io.*;

class Codechef
{
	public static void main (String[] args) throws java.lang.Exception
	{
		// your code goes here
		Scanner in=new Scanner(System.in);
		int t=in.nextInt();
		while(t-->0)
		{
		    int chef=in.nextInt();
		    int chefina=in.nextInt();
		    int steps=in.nextInt();
		    
		    int result=Math.abs(chef-chefina);
		    if(result%steps==0)
		        System.out.println(result/steps);
		    else
		        System.out.println((result/steps)+1);
		}

	}
}
```
