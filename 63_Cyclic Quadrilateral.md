# Cyclic Quadrilateral

Read problem statements in Mandarin Chinese, Russian, and Vietnamese as well.

You are given the sizes of angles of a simple quadrilateral (in degrees) AA, BB, CC and DD, in some order along its perimeter. Determine whether the quadrilateral is cyclic.

Note: A quadrilateral is cyclic if and only if the sum of opposite angles is 180∘180∘. Input

The first line of the input contains a single integer TT denoting the number of test cases. The description of TT test cases follows.
The first and only line of each test case contains four space-separated integers AA, BB, CC and DD.

# Java
```java

import java.util.*;
import java.lang.*;
import java.io.*;

class Codechef
{
	public static void main (String[] args) throws java.lang.Exception
	{
		Scanner sc=new Scanner(System.in);
		int t=sc.nextInt();
		while(t>0)
		{
		    int a=sc.nextInt();
		    int b=sc.nextInt();
		    int c=sc.nextInt();
		    int d=sc.nextInt();
		    
		        
		       if(a+c==180)
		      {
		          if(b+d==180)
		              System.out.println("YES");
		          else
		             System.out.println("NO");
		      }
		    else
		         System.out.println("NO");
		    t--;   
		}
	}
}
```
