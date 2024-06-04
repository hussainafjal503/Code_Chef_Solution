# Presents for Cheffina

Chef has fallen in love with Cheffina, and wants to buy NN gifts for her. On reaching the gift shop, Chef got to know the following two things:

    The cost of each gift is 11 coin.
    On the purchase of every 4th4th gift, Chef gets the 5th5th gift free of cost.

What is the minimum number of coins that Chef will require in order to come out of the shop carrying NN gifts?
Input Format

    The first line of input will contain an integer TT — the number of test cases. The description of TT test cases follows.
    The first and only line of each test case contains an integer NN, the number of gifts in the shop.

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
		    int coin=(n/5)*4+(n%5);
		    System.out.println(coin);
		}

	}
}
```
