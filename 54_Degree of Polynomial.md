# Degree of Polynomial

In mathematics, the degree of polynomials in one variable is the highest power of the variable in the algebraic expression with non-zero coefficient.

Chef has a polynomial in one variable xx with NN terms. The polynomial looks like A0⋅x0+A1⋅x1+…+AN−2⋅xN−2+AN−1⋅xN−1A0​⋅x0+A1​⋅x1+…+AN−2​⋅xN−2+AN−1​⋅xN−1 where Ai−1Ai−1​ denotes the coefficient of the ithith term xi−1xi−1 for all (1≤i≤N)(1≤i≤N).

Find the degree of the polynomial.

Note: It is guaranteed that there exists at least one term with non-zero coefficient.
Input Format

    First line will contain TT, number of test cases. Then the test cases follow.
    First line of each test case contains of a single integer NN - the number of terms in the polynomial.
    Second line of each test case contains of NN space-separated integers - the ithith integer Ai−1Ai−1​ corresponds to the coefficient of xi−1xi−1.

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
		int x=in.nextInt();
		while(x-->0)
		{
		    int size=in.nextInt();
		    int p=0;
		    int []arr =new int[size];
		    for(int i=0;i<size;i++)
		    {
		        arr[i]=in.nextInt();
		        if(arr[i]!=0)
		            p=i;
		        
		    }
		    System.out.println(p);
		}
		

	}
}
```
