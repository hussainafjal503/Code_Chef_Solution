# Valentine is Coming

Valentine's Day is approaching and thus Chef wants to buy some chocolates for someone special.

Chef has a total of XX rupees and one chocolate costs YY rupees. What is the maximum number of chocolates Chef can buy?
Input Format

    First line will contain TT, the number of test cases. Then the test cases follow.
    Each test case contains a single line of input, two integers X,YX,Y - the amount Chef has and the cost of one chocolate respectively.

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
		    int rupees=in.nextInt();
		    int chocolate=in.nextInt();
		    System.out.println(rupees/chocolate);
		}

	}
}
```
