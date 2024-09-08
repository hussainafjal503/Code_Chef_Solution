# Cup Finals

It is the World Cup Finals. Chef only finds a match interesting if the skill difference of the competing teams is less than or equal to DD.

Given that the skills of the teams competing in the final are XX and YY respectively, determine whether Chef will find the game interesting or not. Input Format

The first line of input will contain a single integer TT, denoting the number of testcases. The description of TT testcases follows.
Each testcase consists of a single line of input containing three space-separated integers XX, YY, and DD — the skill levels of the teams and the maximum skill difference.

# Java
```java
/* package codechef; // don't place package name! */

import java.util.*;
import java.lang.*;
import java.io.*;

/* Name of the class has to be "Main" only if the class is public. */
class Codechef
{
	public static void main (String[] args) throws java.lang.Exception
	{
		// your code goes here
		Scanner sc = new Scanner (System.in);
		 int t =sc.nextInt();
		 while(t-->0){
		     int a = sc.nextInt();
		     int b = sc.nextInt();
		     int d = sc.nextInt();
		     
		     if(Math.abs(a-b)<=d){
		         System.out.println("Yes");
		     }
		     else{
		         System.out.println("No");
		     }
		     
		 }
	}
}
```
