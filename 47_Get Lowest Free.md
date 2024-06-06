# Get Lowest Free

Chef goes to the supermarket to buy some items. Luckily there's a sale going on under which Chef gets the following offer:

    If Chef buys 33 items then he gets the item (out of those 33 items) having the lowest price as free.

For e.g. if Chef bought 33 items with the cost 66, 22 and 44, then he would get the item with cost 22 as free. So he would only have to pay the cost of the other two items which will be 6+4=106+4=10.

Chef buys 33 items having prices AA, BB and CC respectively. What is the amount of money Chef needs to pay?

Input Format

    The first line will contain an integer TT - number of test cases. Then the test cases follow.
    The first and only line of each test case contains three integers A,B,CA,B,C - the prices of the items bought by Chef.

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
	        int []arr=new int[3];
	        for(int i=0;i<arr.length;i++)
	            arr[i]=in.nextInt();
	   
	        Arrays.sort(arr);
	        
	        int sum=arr[1]+arr[2];
	        System.out.println(sum);
	    }

	}
}
```
