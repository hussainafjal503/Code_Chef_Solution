# Building Race

Two friends Chef and Chefina are currently on floors AA and BB respectively. They hear an announcement that prizes are being distributed on the ground floor and so decide to reach the ground floor as soon as possible.

Chef can climb down XX floors per minute while Chefina can climb down YY floors per minute. Determine who will reach the ground floor first (ie. floor number 0). In case both reach the ground floor together, print Both.
Input Format

    The first line of input will contain a single integer TT, denoting the number of test cases.
    The first line of each test case contains four space-separated integers AA, BB, XX, and YY — the current floor of Chef, the current floor of Chefina, speed of Chef and speed of Chefina in floors per minute respectively.

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
		    double a=in.nextInt();
		    double b=in.nextInt();
		    double x=in.nextInt();
		    double y=in.nextInt();
		    if((a/x)<(b/y))
		        System.out.println("Chef");
		    else if((a/x)==(b/y))
		        System.out.println("Both");
		    else
		        System.out.println("Chefina");
		}

	}
}
```
