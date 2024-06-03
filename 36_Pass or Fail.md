# Pass or Fail

Chef is struggling to pass a certain college course.

The test has a total of NN questions, each question carries 33 marks for a correct answer and −1−1 for an incorrect answer. Chef is a risk-averse person so he decided to attempt all the questions. It is known that Chef got XX questions correct and the rest of them incorrect. For Chef to pass the course he must score at least PP marks.

Will Chef be able to pass the exam or not?
Input Format

    First line will contain TT, number of testcases. Then the testcases follow.
    Each testcase contains of a single line of input, three integers N,X,PN,X,P.

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
		    int n,x,p;
		   n=in.nextInt();
		   x=in.nextInt();
		   p=in.nextInt();
		  if((x*3)-(n-x)>=p)
		    System.out.println("PAss");
		  else
		    System.out.println("Fail");
		}

	}
}
```
