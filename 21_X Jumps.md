# X Jumps

Chef is currently standing at stair 00 and he wants to reach stair numbered XX.

Chef can climb either YY steps or 11 step in one move.
Find the minimum number of moves required by him to reach exactly the stair numbered XX.
Input Format

    The first line of input will contain a single integer TT, denoting the number of test cases.
    Each test case consists of a single line of input containing two space separated integers XX and YY denoting the number of stair Chef wants to reach and the number of stairs he can climb in one move.

Output Format

For each test case, output the minimum number of moves required by him to reach exactly the stair numbered XX.
Constraints

    1≤T≤5001≤T≤500
    1≤X,Y≤1001≤X,Y≤100

Sample 1:
Input
Output

4
4 2
8 3
3 4
2 1

2
4
3
2
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
		    int stair=in.nextInt();
		    int jump=in.nextInt();
		    System.out.println((stair/jump)+(stair%jump));
		}
	}
}
```
