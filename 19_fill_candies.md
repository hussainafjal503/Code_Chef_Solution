# Fill Candies

Chef received NN candies on his birthday. He wants to put these candies in some bags. A bag has KK pockets and each pocket can hold at most MM candies. Find the minimum number of bags Chef needs so that he can put every candy into a bag.
Input Format

    The first line of input will contain a single integer TT, denoting the number of test cases.
    Each test case consists of a single line containing three space-separated integers N,K,MN,K,M.

output: -
Sample 1:
Input
Output

4
6 2 3
3 1 2
8 4 1
25 4 2

1
2
2
4
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
		    int candies=in.nextInt();
		    int packet=in.nextInt();
		    int Mcandy=in.nextInt();
		    if(candies%(packet*Mcandy)==0)
		        System.out.println(candies/(packet*Mcandy));
		    else
		        System.out.println(candies/(packet*Mcandy)+1);
		    
		}

	}
}
```
