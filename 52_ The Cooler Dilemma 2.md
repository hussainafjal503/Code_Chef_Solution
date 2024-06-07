# The Cooler Dilemma 2

The summer is at its peak in Chefland. Chef is planning to purchase a water cooler to keep his room cool. He has two options available:

    Rent a cooler at the cost of XX coins per month.
    Purchase a cooler for YY coins.

Chef wonders what is the maximum number of months for which he can rent the cooler such that the cost of renting is strictly less than the cost of purchasing it.
Input Format

    The first line of input will contain an integer TT — the number of test cases. The description of TT test cases follows.
    The first and only line of each test case contains two integers XX and YY, as described in the problem statement.

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
		    int x=in.nextInt();
		    int y=in.nextInt();
		    if(y%x!=0)
		        System.out.println(y/x);
		    else
		        System.out.println((y/x)-1);
		}

	}
}
```
