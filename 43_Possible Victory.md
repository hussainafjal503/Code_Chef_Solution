# Possible Victory

Chef is playing in a T20 cricket match. In a match, Team A plays for 20 overs. In a single over, the team gets to play 6 times, and in each of these 6 tries, they can score a maximum of 6 runs. After Team A's 20 overs are finished, Team B similarly plays for 20 overs and tries to get a higher total score than the first team. The team with the higher total score at the end wins the match.

Chef is in Team B. Team A has already played their 20 overs, and have gotten a score of RR. Chef's Team B has started playing, and have already scored CC runs in the first OO overs. In the remaining 20−O20−O overs, find whether it is possible for Chef's Team B to get a score high enough to win the game. That is, can their final score be strictly larger than RR?

Input Format

  There is a single line of input, with three integers, R,O,CR,O,C.
```java

import java.util.*;
import java.lang.*;
import java.io.*;

class Codechef
{
	public static void main (String[] args) throws java.lang.Exception
	{
		// your code goes here
		Scanner in= new Scanner (System.in);
		int r=in.nextInt();
		int over=in.nextInt();
		int score=in.nextInt();
		if(r<score+(((20-over)*6)*6))
            System.out.println("Yes");
        else
            System.out.println("No");
		
		

	}
}
```
