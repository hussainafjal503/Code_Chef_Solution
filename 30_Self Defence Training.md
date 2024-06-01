# Self Defence Training

After the phenomenal success of the 36th Chamber of Shaolin, San Te has decided to start 37th Chamber of Shaolin. The aim this time is to equip women with shaolin self-defence techniques.

The only condition for a woman to be eligible for the special training is that she must be between 1010 and 6060 years of age, inclusive of both 1010 and 6060.

Given the ages of NN women in his village, please help San Te find out how many of them are eligible for the special training.
Input Format

    The first line of input contains a single integer TT, denoting the number of test cases. The description of TT test cases follows.
    The first line of each test case contains a single integer NN, the number of women.
    The second line of each test case contains NN space-separated integers A1,A2,...,ANA1​,A2​,...,AN​, the ages of the women.

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
		    int []arr=new int[n];
		    
		    for(int i=0;i<arr.length;i++)
		        arr[i]=in.nextInt();
		        
		    int count=0; 
		    for(int i=0;i<arr.length;i++)
		    {
		        if(arr[i]>=10 && arr[i]<=60)
		            count++;
		    }
		    System.out.println(count);
		}

	}
}
```
