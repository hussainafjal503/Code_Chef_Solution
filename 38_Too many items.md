# Too many items

Chef bought NN items from a shop. Although it is hard to carry all these items in hand, so Chef has to buy some polybags to store these items.

11 polybag can contain at most 1010 items. What is the minimum number of polybags needed by Chef?
Input Format

    The first line will contain an integer TT - number of test cases. Then the test cases follow.
    The first and only line of each test case contains an integer NN - the number of items bought by Chef.

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
		    int n=in.nextInt();
		    if(n%10==0)
		        System.out.println(n/10);
		    else
		        System.out.println((n/10)+1);
		}

	}
}
```
