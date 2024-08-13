# ATM Machine

###Read problems statements Bengali , Mandarin chinese , Russian and Vietnamese as well.

There is an ATM machine. Initially, it contains a total of KK units of money. NN people (numbered 11 through NN) want to withdraw money; for each valid ii, the ii-th person wants to withdraw AiAi​ units of money.

The people come in and try to withdraw money one by one, in the increasing order of their indices. Whenever someone tries to withdraw money, if the machine has at least the required amount of money, it will give out the required amount. Otherwise, it will throw an error and not give out anything; in that case, this person will return home directly without trying to do anything else.

For each person, determine whether they will get the required amount of money or not. Input

The first line of the input contains a single integer TT denoting the number of test cases. The description of TT test cases follows.
The first line of each test case contains two space-separated integers NN and KK.
The second line contains NN space-separated integers A1,A2,…,ANA1​,A2​,…,AN​.

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
		    int k=in.nextInt();
		    int [] arr=new int[n];
		    for(int i=0;i<arr.length;i++)
		        arr[i]=in.nextInt();
		    
		    
		    for(int i=0;i<arr.length;i++)
		    {
		        if(arr[i]<=k)
		        {
		            System.out.print("1");
		            k=k-arr[i];
		        }
		        else
		            System.out.print("0");
		    }
		    System.out.println();
		}
	}
}
```
