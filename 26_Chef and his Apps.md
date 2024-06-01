# Chef and his Apps

Chef's phone has a total storage of SS MB. Also, Chef has 22 apps already installed on his phone which occupy XX MB and YY MB respectively.

He wants to install another app on his phone whose memory requirement is ZZ MB. For this, he might have to delete the apps already installed on his phone. Determine the minimum number of apps he has to delete from his phone so that he has enough memory to install the third app.
Input Format

    The first line contains a single integer TT — the number of test cases. Then the test cases follow.
    The first and only line of each test case contains four integers S,X,YS,X,Y and ZZ — the total memory of Chef's phone, the memory occupied by the two already installed apps and the memory required by the third app.

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
		    int t_memory=in.nextInt();
		    int ocu1=in.nextInt();
		    int ocu2=in.nextInt();
		    int req=in.nextInt();
		    if(t_memory-req>=ocu1+ocu2 && t_memory>=ocu1+ocu2+req)
		        System.out.println(0);
		    else if(t_memory==req || t_memory<ocu1+req)
		        System.out.println(2);
		    else
		        System.out.println(1);
		    
		}

	}
}
```
