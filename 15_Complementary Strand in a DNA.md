# Complementary Strand in a DNA

You are given the sequence of Nucleotides of one strand of DNA through a string SS of length NN. SS contains the character A,T,C,A,T,C, and GG only.

Chef knows that:
    AA is complementary to TT.
    TT is complementary to AA.
    CC is complementary to GG.
    GG is complementary to CC.

Using the string SS, determine the sequence of the complementary strand of the DNA.

Input Format
    First line will contain TT, number of test cases. Then the test cases follow.
    First line of each test case contains an integer NN - denoting the length of string SS.
    Second line contains NN characters denoting the string SS.

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
		    int length=in.nextInt();
		    String ch=in.next();
		    
		    for(int i=0;i<length;i++)
		    {
		        if(ch.charAt(i)=='A')
		            System.out.print("T");
		        else if(ch.charAt(i)=='T')
		            System.out.print("A");
		        else if(ch.charAt(i)=='C')
		            System.out.print("G");
		        else
		            System.out.print("C");
		    }
		    System.out.println();
		   
		    
		}

	}
}
```
