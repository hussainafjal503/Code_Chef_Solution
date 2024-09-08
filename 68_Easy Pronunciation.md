# Easy Pronunciation

Words that contain many consecutive consonants, like "schtschurowskia", are generally considered somewhat hard to pronounce.

We say that a word is hard to pronounce if it contains 44 or more consonants in a row; otherwise it is easy to pronounce. For example, "apple" and "polish" are easy to pronounce, but "schtschurowskia" is hard to pronounce.

You are given a string SS consisting of NN lowercase Latin characters. Determine whether it is easy to pronounce or not based on the rule above — print YES if it is easy to pronounce and NO otherwise.

For the purposes of this problem, the vowels are the characters {a,e,i,o,u}{a,e,i,o,u} and the consonants are the other 2121 characters. Input Format

The first line of input will contain a single integer TT, denoting the number of test cases.
Each test case consists of two lines of input.
    The first line of each test case contains a single integer NN, the length of string SS.
    The second line of each test case contains the string SS.

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
		   int count=0;
		  int n=in.nextInt();
		  String s=in.next();
		  s.toLowerCase();
		  if(n<4)
		  {
		    System.out.println("YES");
		  }
		  else{
		      
		  
		  for(int i=0;i<s.length();i++)
		  {
		      if(count==4)
		            break;
		            
		      if(s.charAt(i)=='a'|| s.charAt(i)=='e'|| s.charAt(i)=='i'|| s.charAt(i)=='o'|| s.charAt(i)=='u')
		            count=0;
		        else 
		            count++;;
		      
		  }
		  if(count==4)
		        System.out.println("No");
		    else
		    System.out.println("YES");
		  }
		}

	}
}
```
