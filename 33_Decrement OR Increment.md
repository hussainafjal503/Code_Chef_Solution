# Decrement OR Increment

Write a program to obtain a number NN and increment its value by 1 if the number is divisible by 4 otherwiseotherwise decrement its value by 1.
Input Format

First line will contain a number NN.

```java
import java.util.*;
import java.lang.*;
import java.io.*;

class Codechef
{
	public static void main (String[] args) throws java.lang.Exception
	{
		// your code goes here
		Scanner in = new Scanner(System.in);
		int n= in.nextInt();
		if(n%4==0)
		    System.out.println(++n);
		else
		    System.out.println(--n);

	}
}
```
