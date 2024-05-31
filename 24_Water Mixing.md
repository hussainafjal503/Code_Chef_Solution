# Water Mixing

Chef is setting up a perfect bath for himself. He has XX litres of hot water and YY litres of cold water.
The initial temperature of water in his bathtub is AA degrees. On mixing water, the temperature of the bathtub changes as following:

    The temperature rises by 11 degree on mixing 11 litre of hot water.
    The temperature drops by 11 degree on mixing 11 litre of cold water.

Determine whether he can set the temperature to BB degrees for a perfect bath.
Input Format

    The first line of input will contain a single integer TT, denoting the number of test cases.
    Each test case consists of four space-separated integers A,B,X,A,B,X, and YY — the initial temperature of bathtub, the desired temperature of bathtub, the amount of hot water in litres, and the amount of cold water in litres respectively.

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
		    int a_degree=in.nextInt();
		    int b_degree=in.nextInt();
		    int hot=in.nextInt();
		    int cold=in.nextInt();
		    if(a_degree==b_degree)
		        System.out.println("Yes");
		    else
		    {
		        if(a_degree<b_degree)
		        {
		           a_degree+=hot;
		           if(a_degree>=b_degree)
		                System.out.println("Yes");
		            else
		                System.out.println("No");
		        }
		        else
		        {
		            if(a_degree>b_degree)
		            {
		                b_degree+=cold;
		                if(b_degree>=a_degree)
		                    System.out.println("Yes");
		                else
		                    System.out.println("No");
		                
		            }
		        }
		    }
		}

	}
}
```
