# Pass or Fail

Chef is struggling to pass a certain college course.

The test has a total of NN questions, each question carries 33 marks for a correct answer and −1−1 for an incorrect answer. Chef is a risk-averse person so he decided to attempt all the questions. It is known that Chef got XX questions correct and the rest of them incorrect. For Chef to pass the course he must score at least PP marks.

Will Chef be able to pass the exam or not? Input Format

First line will contain TT, number of testcases. Then the testcases follow.
Each testcase contains of a single line of input, three integers N,X,PN,X,P.

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
		Scanner sc= new Scanner(System.in);
		int n= sc.nextInt();
		for (int i=0;i<n;i++){
		    int x = sc.nextInt();
		    int y = sc.nextInt();
		    int z = sc.nextInt();
		    
		    int marks=(y*3)-(x-y);
		    if(marks>=z)
		        System.out.println("PASS");
		    else
		        System.out.println("FAIL");
		}
	}
}
```
