# Chef Eren

Chef is a very big fan of Eren Yeager.

In the last season of Attack on Titan, there were NN episodes numbered from 11 to NN.
Each even indexed episode was AA minutes long and each odd indexed episode was BB minutes long.

Calculate the total duration (in minutes) of the last season.
Input Format

    The first line of input contains a single integer TT, the number of test cases.
    The first and only line of each test case contains three integers NN, A,A, and BB, the number of episodes and the durations of each even-indexed and odd-indexed episodes respectively in minutes.

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
		    int n=in.nextInt();
		    int even=in.nextInt();
		    int odd=in.nextInt();
		    int e=0,o=0;
		    for(int i=1;i<=n;i++)
		    {
		        if(i%2!=0)
		            o++;
		        else
		            e++;
		    }
		    if(n==1)
		        System.out.println(o*odd);
		    else
		    {
		        System.out.println((o*odd)+(e*even));
		    }
		}

	}
}
```
