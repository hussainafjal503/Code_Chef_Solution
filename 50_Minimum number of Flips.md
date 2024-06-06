# Minimum number of Flips

Chef has an array AA of length NN consisting of 11 and −1−1 only.

In one operation, Chef can choose any index ii (1≤i≤N)(1≤i≤N) and multiply the element AiAi​ by −1−1.

Find the minimum number of operations required to make the sum of the array equal to 00. Output -1 if the sum of the array cannot be made 00.
Input Format

  First line will contain TT, number of test cases. Then the test cases follow.
  First line of each test case consists of a single integer NN denoting the length of the array.
  Second line of each test case contains NN space-separated integers A1,A2,…,ANA1​,A2​,…,AN​ denoting the array AA.

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
		    int arr[]=new int[n];
		    for(int i=0;i<n;i++)
		        arr[i]=in.nextInt();
		    
		    
		    if(n%2==0)
		    {
		        int d = n/2;
		        int c = 0;
		        for(int i = 0; i<arr.length; i++)
		        {
		            if(arr[i]==-1)
		                c++;
		        }
		            
		        
		        int e = Math.abs(d-c);
		        System.out.println(e);
		    
		        
		    }
		    
		    else
		        System.out.println(-1);
		}

	}
}
```
