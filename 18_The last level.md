# The Last Levels

Chef is playing a videogame, and is getting close to the end. He decides to finish the rest of the game in a single session.

There are XX levels remaining in the game, and each level takes Chef YY minutes to complete. To protect against eye strain, Chef also decides that every time he completes 33 levels, he will take a ZZ minute break from playing. Note that there is no need to take this break if the game has been completed.

How much time (in minutes) will it take Chef to complete the game?

Input Format: -

  The first line of input will contain a single integer TT, denoting the number of test cases.
  The first and only line of input will contain three space-separated integers XX, YY, and ZZ.

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
		    int z=in.nextInt();
		    if(x<=3)
		        System.out.println(y*x);
		    else if(x%3==0)
		        System.out.println(x*y+((x/3-1)*z));
		    else
		          System.out.println(x*y+((x/3)*z));
		}

	}
}
```
