# Primality Test

Alice and Bob are meeting after a long time. As usual they love to play some math games. This times Alice takes the call and decides the game. The game is very simple, Alice says out an integer and Bob has to say whether the number is prime or not. Bob as usual knows the logic but since Alice doesn't give Bob much time to think, so Bob decides to write a computer program.

Help Bob accomplish this task by writing a computer program which will calculate whether the number is prime or not.

Note that 1 is not a prime number.

Input

The first line of the input contains an integer T, the number of testcases. T lines follow.

Each of the next T lines contains an integer N which has to be tested for primality. 

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
		    int count=0;
		    if(n==1)
		        System.out.println("no");
		    else
		    {
		        for(int i=2;i<=n/2;i++)
		        {
		            if(n%i==0)
		            {
		                count++;
		                break;
		            }
		           
		        }
		        if(count==0)
		            System.out.println("yes");
		        else
		            System.out.println("no");
		    }
		    
		}

	}
}
```
