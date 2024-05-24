
 # Chess Ratings

Alice has recently started playing Chess. Her current rating is XX. She noticed that when she wins a game, her rating increases by 88 points.

Can you help Alice in finding out the minimum number of games she needs to win in order to make her rating greater than or equal to YY?

Input Format

The first line of input will contain an integer TT — the number of test cases. The description of TT test cases follows.
The first line of each test case contains two integers XX and YY, as described in the problem statement.


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
	        int x=in.nextInt();
	        int y=in.nextInt();
	        int count=0;
	        if(x==y)
	            System.out.println(0);
	       else
	       {
	           while(y>x)
	           {
	               x=x+8;
	               count+=1;
	               if(x>=y)
	                    break;
	           }
	           System.out.println(count);
	       }
	    }

	}
}
```
