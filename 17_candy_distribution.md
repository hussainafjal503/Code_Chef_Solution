# Candy Distribution

Chef has NN candies. He has to distribute them to exactly MM of his friends such that each friend gets equal number of candies and each friend gets even number of candies. Determine whether it is possible to do so.

NOTE: Chef will not take any candies himself and will distribute all the candies.
Input Format: -

  First line will contain TT, number of test cases. Then the test cases follow.
  Each test case contains of a single line of input, two integers NN and MM, the number of candies and the number of friends.

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
		    int candies=in.nextInt();
		    int friends=in.nextInt();
		    if(candies%friends==0 && (candies/friends)%2==0)
		        System.out.println("YES");
		        
		    else
		        System.out.println("NO");
		}

	}
}
```
