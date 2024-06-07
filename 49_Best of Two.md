# Best of Two

Alice and Bob are playing a game. Each player rolls a regular six faced dice 33 times.
The score of a player is the sum of the values of the highest 22 rolls. The player with the highest score wins, and the game ends in a Tie if both players have the same score.

Find the winner of the game or determine whether it is a tie.
Input Format

  The first line of input will contain a single integer TT, denoting the number of test cases.
  Each test case contains six space-separated integers A1A1​, A2A2​, A3A3​, B1B1​, B2B2​ and B3B3​ — the values Alice gets in her 33 dice rolls, followed by the values which Bob gets in his 33 dice rolls.
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
		    int [][]arr=new int[2][3];
		    for(int i=0;i<arr.length;i++)
		    {
		        for(int j=0;j<arr[i].length;j++)
		            arr[i][j]=in.nextInt();
		    }
		        
		  
		    int alice=0,bob=0;
		  
		    Arrays.sort(arr[0]);
		    Arrays.sort(arr[1]);
		    
		   alice=arr[0][2]+arr[0][1];
		   bob=arr[1][2]+arr[1][1];
		    
		    
		    if(alice>bob)
		        System.out.println("Alice");
		    else if(alice<bob)
		        System.out.println("Bob");
		    else
		        System.out.println("Tie");
		}

	}
}
```
