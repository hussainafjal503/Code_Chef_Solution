# Cyclic Quadrilateral
Read problem statements in Mandarin Chinese, Russian, and Vietnamese as well.

You are given the sizes of angles of a simple quadrilateral (in degrees) AA, BB, CC and DD, in some order along its perimeter. Determine whether the quadrilateral is cyclic.

Note: A quadrilateral is cyclic if and only if the sum of opposite angles is 180∘180∘.
Input

    The first line of the input contains a single integer TT denoting the number of test cases. The description of TT test cases follows.
    The first and only line of each test case contains four space-separated integers AA, BB, CC and DD.
```java
import java.util.*;
import java.lang.*;
import java.io.*;

class Codechef
{
	public static void main (String[] args) throws java.lang.Exception
	{
		// your code goes here
		Scanner in=new Scanner (System.in);
	    int t=in.nextInt();
	    while(t-->0)
	    {
	        int a=in.nextInt();
	        int b=in.nextInt();
	        int c=in.nextInt();
	        int d=in.nextInt();
	        if(a+c==180 || b+d==180)
	            System.out.println("Yes");
	        else
	            System.out.println("No");
	    }

	}
}
```
