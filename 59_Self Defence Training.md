# Self Defence Training

After the phenomenal success of the 36th Chamber of Shaolin, San Te has decided to start 37th Chamber of Shaolin. The aim this time is to equip women with shaolin self-defence techniques.

The only condition for a woman to be eligible for the special training is that she must be between 1010 and 6060 years of age, inclusive of both 1010 and 6060.

Given the ages of NN women in his village, please help San Te find out how many of them are eligible for the special training. Input Format

The first line of input contains a single integer TT, denoting the number of test cases. The description of TT test cases follows.
The first line of each test case contains a single integer NN, the number of women.
The second line of each test case contains NN space-separated integers A1,A2,...,ANA1​,A2​,...,AN​, the ages of the women.

# Java
```java
/* package codechef; // don't place package name! */

import java.util.*;
import java.lang.*;
import java.io.*;

/* Name of the class has to be "Main" only if the class is public. */
class Codechef
{
	public static void main (String[] args) throws java.lang.Exception
	{
	    int count = 0 ;
	    Scanner sc = new Scanner(System.in);
	    int T = sc.nextInt();
	    while(T!=0)
	    {
	        int N = sc.nextInt();
	        while(N!=0)
	        {
	            int A = sc.nextInt();
	            if(A>=10 &&A<=60)
	                count++;
	            
	            N--;
	        }
	        System.out.println(count);
	        count =  0; 
	        
	        T--;
	    }
		// your code goes here
	}
}
```
