# Candies

Abhi is a salesman. He was given two types of candies, which he is selling in NN different cities.

For the prices of the candies to be valid, Abhi's boss laid down the following condition:

A given type of candy must have distinct prices in all NN cities.

In his excitement, Abhi wrote down the prices of both the candies on the same page and in random order instead of writing them on different pages. Now he is asking for your help to find out if the prices he wrote are valid or not.

You are given an array AA of size 2N2N. Find out whether it is possible to split AA into two arrays, each of length NN, such that both arrays consist of distinct elements.

Both arrays can have distinct elements only if no element in the original array is repeated more than twice. Input Format

The first line of input will contain a single integer TT, denoting the number of test cases.
Each test case consists of two lines of input.
    The first line of each test case contains one integer NN, denoting the number of cities
    The second line contains 2N2N space-separated integers A1,A2,…,A2NA1​,A2​,…,A2N​ — the elements of the array AA.

    Output Format

For each test case output the answer on a new line — Yes if the given array represents a valid list of prices, and No otherwise.

Each letter of the output may be printed in either uppercase or lowercase, i.e, Yes, YES, and yEs will all be treated as equivalent.

# Java
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
            int[]arr=new int[n*2];
            int count=0;
            
            for(int i=0;i<n*2;i++)
                arr[i]=in.nextInt();
            
            
            for(int i=0;i<arr.length;i++)
            {
                count=0;
                for(int j=i;j<arr.length;j++)
                {
                    if(arr[i]==arr[j])
                        count++;
                   
                }
                if(count>2)
                    break;
            }
            if(count<2)
                System.out.println("YES");
            else
                System.out.println("NO");   
            
        }
	  }
}
```
