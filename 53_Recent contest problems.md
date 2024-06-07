# Recent contest problems

CodeChef recently revamped its practice page to make it easier for users to identify the next problems they should solve by introducing some new features:

    Recent Contest Problems - Contains only problems from the last 2 contests
    Separate Un-Attempted, Attempted, and All tabs
    Problem Difficulty Rating - The Recommended dropdown menu has various difficulty ranges so that you can attempt the problems most suited to your experience
    Popular Topics and Tags

Chef has been participating regularly in rated contests but missed the last two contests due to his college exams. He now wants to solve them and so he visits the practice page to view these problems.

Given a list of NN contest codes, where each contest code is either START38 or LTIME108, help Chef count how many problems were featured in each of the contests.
Input Format

    First line will contain TT, number of test cases. Then the test cases follow.
    Each test case contains of two lines of input.
    First line of input contains the total count of problems that appeared in the two recent contests - NN.
    Second line of input contains the list of NN contest codes. Each code is either START38 or LTIME108, to which each problem belongs.

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
		    int n=in.nextInt();
		    String []arr=new String[n];
		    int c1=0,c2=0;
		    for(int i=0;i<n;i++)
		    {
		       arr[i]=in.next();
		    }
		    
		    for(int i =0;i<arr.length;i++)
		    {
		        if(arr[i].equalsIgnoreCase("start38"))
		            c1++;
		        else
		            c2++;
		    }
		    System.out.println(c1+" "+c2);
		}

	}
}
```
