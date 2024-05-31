# Weights

Chef is playing with weights. He has an object weighing WW units. He also has three weights each of X,Y,X,Y, and ZZ units respectively. Help him determine whether he can measure the exact weight of the object with one or more of these weights.

If it is possible to measure the weight of object with one or more of these weights, print YES, otherwise print NO.
Input Format

    The first line of input will contain a single integer TT, denoting the number of test cases.
    Each test case consists of single line containing a four positive integers W,X,Y,W,X,Y, and ZZ.

Output Format

For each test case, output on a new line YES if it is possible to measure the weight of object with one or more of these weights, otherwise print NO.

You may print each character of the string in either uppercase or lowercase (for example, the strings yes, YES, Yes, and yeS will all be treated as identical).
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
		    int object=in.nextInt();
		    int x=in.nextInt();
		    int y=in.nextInt();
		    int z=in.nextInt();
		    if(object==x || object==y || object==z)
		        System.out.println("Yes");
		    else
		    {
		        int w1=x+y;
		        int w2=x+z;
		        int w3=y+z;
		        int w4=x+y+z
		        if(w1==object || w2==object || w3==object || w4==object)
		            System.out.println("Yes");
		        else
		            System.out.println("No");
		    }
		}

	}
}
```
