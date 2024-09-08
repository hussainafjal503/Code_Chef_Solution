# Break the Stick

Chef has a stick of length NN.

He can break the stick into 22 or more parts such that the parity of length of each part is same. For example, a stick of length 1111 can be broken into three sticks of lengths {3,3,5}{3,3,5} since each part is odd, but it cannot be broken into two sticks of lengths {5,6}{5,6} since one is even and the other is odd.

Chef can then continue applying this operation on the smaller sticks he obtains, as many times as he likes.

Can Chef obtain a stick of length exactly XX by doing this? Input Format

The first line of input will contain a single integer TT, denoting the number of test cases. The description of the test cases follows.
Each test case consists of a single line of input, containing two space-separated integers N,XN,X.

Output Format

For each test case, output on a new line YES if Chef can obtain a stick of length exactly XX, and NO otherwise.

Each letter of the output may be printed in either lowercase or uppercase. For example, the strings YES, yEs, and Yes will be considered identical.

# Java
```java
java
import java.util.*;
import java.lang.*;
import java.io.*;

class Codechef
{
	public static void main (String[] args) throws java.lang.Exception
	{
		// your code goes here
		Scanner in =new Scanner (System.in);
		int t=in.nextInt();
		while(t-->0)
		{
		    int x=in.nextInt();
		    int y=in.nextInt();
		    
		    
		    if(x%2==0)
		        System.out.println("YES");
		    else if(y%2==0)
		        System.out.println("NO");
		    else
		        System.out.println("YES");
		}

	}
}
```
