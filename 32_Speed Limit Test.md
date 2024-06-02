# Speed Limit Test

Alice is driving from her home to her office which is AA kilometers away and will take her XX hours to reach.
Bob is driving from his home to his office which is BB kilometers away and will take him YY hours to reach.

Determine who is driving faster, else, if they are both driving at the same speed print EQUAL.
Input Format

    The first line will contain TT, the number of test cases. Then the test cases follow.
    Each test case consists of a single line of input, containing four integers A,X,B,A,X,B, and YY, the distances and and the times taken by Alice and Bob respectively.

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
		   double alice=in.nextInt();
		   double x=in.nextInt();
		   double bob=in.nextInt();
		   double y=in.nextInt();
		    if((alice/x)<(bob/y))
		        System.out.println("Bob");
		    else if((alice/x)==(bob/y))
		        System.out.println("Equal");
		    else
		        System.out.println("Alice");
		    
		}

	}
}
```
