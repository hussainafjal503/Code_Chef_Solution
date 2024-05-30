# Chessboard Distance

The Chessboard Distance for any two points (X1,Y1)(X1​,Y1​) and (X2,Y2)(X2​,Y2​) on a Cartesian plane is defined as max(∣X1−X2∣,∣Y1−Y2∣)max(∣X1​−X2​∣,∣Y1​−Y2​∣).

You are given two points (X1,Y1)(X1​,Y1​) and (X2,Y2)(X2​,Y2​). Output their Chessboard Distance.

Note that, ∣P∣∣P∣ denotes the absolute value of integer PP. For example, ∣−4∣=4∣−4∣=4 and ∣7∣=7∣7∣=7.
Input Format

    First line will contain TT, the number of test cases. Then the test cases follow.
    Each test case consists of a single line of input containing 44 space separated integers - X1,Y1,X2,Y2X1​,Y1​,X2​,Y2​ - as defined in the problem statement.

Output Format

For each test case, output in a single line the chessboard distance between (X1,Y1)(X1​,Y1​) and (X2,Y2)(X2​,Y2​)
Sample 1:
Input
Output

3
2 4 5 1
5 5 5 3
1 4 3 3

3
2
2
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
		    int a=in.nextInt();
		    int b=in.nextInt();
		    int c=in.nextInt();
		    int d=in.nextInt();
		    int result1=Math.abs(a-c);
		    int result2=Math.abs(b-d);
		    if(result1>result2)
		        System.out.println(result1);
		    else
		        System.out.println(result2);
		    
		}

	}
}
```
