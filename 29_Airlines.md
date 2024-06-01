# Airlines

An airline operates XX aircraft every day. Each aircraft can carry up to 100100 passengers.
One day, NN passengers would like to travel to the same destination. What is the minimum number of new planes that the airline must buy to carry all NN passengers?
Input Format

    The first line of input will contain a single integer TT, denoting the number of test cases.
    Each test case consists of a single line containing two space-separated integers XX and NN — the number of aircraft the airline owns and the number of passengers travelling, respectively.

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
		    int aircraft=in.nextInt();
		    int passenger=in.nextInt();
		    if(aircraft*100>=passenger)
		        System.out.println(0);
		    
		    else
		    {
		        int c=passenger-(aircraft*100);
		        if(c%100==0)
		            System.out.println(c/100);
		        else
		            System.out.println(c/100+1);
		    }
		}

	}
}
```
