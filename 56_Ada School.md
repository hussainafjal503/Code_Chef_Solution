# Ada School

###Read problems statements in Hindi, Mandarin Chinese, Russian, Vietnamese and Bengali as well.

Ada's classroom contains N⋅MN⋅M tables distributed in a grid with NN rows and MM columns. Each table is occupied by exactly one student.

Before starting the class, the teacher decided to shuffle the students a bit. After the shuffling, each table should be occupied by exactly one student again. In addition, each student should occupy a table that is adjacent to that student's original table, i.e. immediately to the left, right, top or bottom of that table.

Is it possible for the students to shuffle while satisfying all conditions of the teacher? Input

The first line of the input contains a single integer TT denoting the number of test cases. The description of TT test cases follows.
The first and only line of each test case contains two space-separated integers NN and MM.

Output

For each test case, print a single line containing the string "YES" if it is possible to satisfy the conditions of the teacher or "NO" otherwise (without quotes).

```
java
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
		    int m=in.nextInt();
		    if(n%2!=0 && m%2!=0)
		        System.out.println("NO");
		    else
		        System.out.println("YES");
		}

	}
}
```
