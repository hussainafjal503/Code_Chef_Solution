# Single-use Attack

Chef is playing a video game, and is now fighting the final boss.

The boss has HH health points. Each attack of Chef reduces the health of the boss by XX.
Chef also has a special attack that can be used at most once, and will decrease the health of the boss by YY.

Chef wins when the health of the boss is ≤0≤0.
What is the minimum number of attacks needed by Chef to win?
Input Format

   The first line of input will contain a single integer TT, denoting the number of test cases.
   The first and only line of each test case will contain three space-separated integers H,X,YH,X,Y — the parameters described in the statement.
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
		    int boss_h=in.nextInt();
		    int x=in.nextInt();
		    int y=in.nextInt();
		    if(boss_h<y)
		    {
	            System.out.println("1");
	            return;
	        }
	        
	       int spl = boss_h-y;
	       int count = spl/x;
	       
	       if(spl - count*x  ==  0)
	            count = count;
	       else
	           count++;
	       
	       int numAttacks = count+1;
	       System.out.println(numAttacks);
		    
		}

	}
}
```
