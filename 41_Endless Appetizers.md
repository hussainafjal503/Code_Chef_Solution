# Endless Appetizers

Life is a like a box of of mozzarella sticks. You never know what you're gonna get, but you can predict with 100 percent accuracy that it will be a mozzarella stick.

Chef's colleague issued a challenge to Chef: "If you eat more than XX mozzarella sticks, I'll give you 3030 rupees for each extra one you eat".
For example, if X=5X=5 and Chef eats 88 sticks, he would receive 9090 rupees because he ate 33 extra sticks.

You know that the restaurant serves YY mozzarella sticks per plate.
You also know that Chef received RR rupees from his colleague as a result of the challenge.

What's the maximum number of plates of mozzarella sticks that Chef could have ordered?

Note:

    Chef won't order a new plate till he finishes eating all the sticks from the previous one.
    However, it's possible that Chef didn't finish all the sticks from the final plate he ordered.
    See the explained examples below for more clarification.

Input Format

    The first line of input will contain a single integer TT, denoting the number of test cases.
    Each test case consists of one line of input, containing three space-separated integers X,Y,X,Y, and RR — the lower limit on the number of sticks, the number of sticks on a single plate, and the money received by Chef.

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
		    int x=in.nextInt();
		    int y=in.nextInt();
		    int r=in.nextInt();
		    if((x+(r/30))%y!=0)
		        System.out.println((x+(r/30))/y+1);
		    else
		        System.out.println((x+(r/30))/y);
		}

	}
}
```
