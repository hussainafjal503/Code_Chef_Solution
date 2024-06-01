# Minimum number of coins

Chef has infinite coins in denominations of rupees 55 and rupees 1010.

Find the minimum number of coins Chef needs, to pay exactly XX rupees. If it is impossible to pay XX rupees in denominations of rupees 55 and 1010 only, print −1−1.
Input Format

    First line will contain TT, number of test cases. Then the test cases follow.
    Each test case contains of a single integer XX.

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
		    if(x%10==0 || x%5==0)
		    {
		        if(x%10==0)
		        System.out.println(x/10);
		        else 
		        {   int coin=x%10;
		    
		        System.out.println((x/10)+1);
		        }
		    }
		    else
		        System.out.println(-1);
		   
		}
	}
}
```
