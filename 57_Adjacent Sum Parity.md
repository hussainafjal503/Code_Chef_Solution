# Adjacent Sum Parity

Chef has an array AA of length NN.

Chef forms a binary array BB of length NN using the parity of the sums of adjacent elements in AA. Formally,

Bi=(Ai+Ai+1) % 2Bi​=(Ai​+Ai+1​)%2 for 1≤i≤N−11≤i≤N−1
BN=(AN+A1) % 2BN​=(AN​+A1​)%2

Here x % yx%y denotes the remainder obtained when xx is divided by yy.

Chef lost the array AA and needs your help. Given array BB, determine whether there exists any valid array AA which could have formed BB. Input Format

The first line contains a single integer TT — the number of test cases. Then the test cases follow.
The first line of each test case contains an integer NN — the size of the array AA.
The second line of each test case contains NN space-separated integers B1,B2,…,BNB1​,B2​,…,BN​ denoting the array BB.

Output Format

For each testcase, output YES if there exists a valid array AA, NO otherwise.

You can print any character in any case. For example YES, Yes, yEs are all considered same.
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
		    int []arr=new int[n];
		    
		    for(int i=0;i<n;i++)
		        arr[i]=in.nextInt();
		  
		    int sum=0;
		    for(int i=0;i<n;i++)
		        sum=sum+arr[i];
		    
		    if(sum%2==0)
		        System.out.println("YES");
		    else
		        System.out.println("NO");
		}

	}
}
```
