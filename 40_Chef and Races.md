# Chef and Races

The National Championships are starting soon. There are 44 race categories, numbered from 11 to 44, that Chef is interested in. Chef is participating in exactly 22 of these categories.

Chef has an arch-rival who is, unfortunately, the only person participating who is better than Chef, i.e, Chef can't defeat the arch-rival in any of the four race categories but can defeat anyone else. Chef's arch-rival is also participating in exactly 22 of the four categories.

Chef hopes to not fall into the same categories as that of the arch-rival.

Given X,Y,A,BX,Y,A,B where X,YX,Y are the races that Chef participates in, and A,BA,B are the races that Chef's arch-rival participates in, find the maximum number of gold medals (first place) that Chef can win.
Input Format

    The first line of input contains an integer TT, denoting the number of testcases. The description of TT testcases follows.
    Each testcase consists of a single line containing four space-separated integers — the values of X,Y,AX,Y,A, and BB respectively.

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
		    int a=in.nextInt();
		    int b=in.nextInt();
		    if((x!=a && y!=b) && (x!=b && y!=a))
		        System.out.println(2);
		    else if(x==a && y==b || x==b && y==a)
		        System.out.println(0);
		    else
		        System.out.println(1);
		}

	}
}
```
