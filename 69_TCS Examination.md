# TCS Examination

Two friends, Dragon and Sloth, are writing a computer science examination series. There are three subjects in this series: DSADSA, TOCTOC, and DMDM. Each subject carries 100100 marks.

You know the individual scores of both Dragon and Sloth in all 33 subjects. You have to determine who got a better rank.

The rank is decided as follows:

The person with a bigger total score gets a better rank
If the total scores are tied, the person who scored higher in DSADSA gets a better rank
If the total score and the DSADSA score are tied, the person who scored higher in TOCTOC gets a better rank
If everything is tied, they get the same rank.

Input Format

The first line of input contains a single integer TT, denoting the number of test cases. The description of TT test cases follows.
The first line of each test case contains three space-separated integers denoting the scores of Dragon in DSADSA, TOCTOC and DMDM respectively.
The second line of each test case contains three space-separated integers denoting the scores of Sloth in DSADSA, TOCTOC and DMDM respectively.

# Java
```java
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
		   int ddsa=in.nextInt();
		   int dtoc=in.nextInt();
		   int  ddm=in.nextInt();
		   
		   
		   
		   int sdsa=in.nextInt();
		   int stoc=in.nextInt();
		   int sdm=in.nextInt();
		    
		   int dsum=ddsa+dtoc+ddm;
		   int ssum=sdsa+stoc+sdm;
		 String result;
		
		if(ssum>dsum)
		    result="SLOTH";
		else if(ssum<dsum)
		    result="DRAGON";
		else
		{
		    if(sdsa>ddsa)
		        result="SLOTH";
		    else if(ddsa>sdsa)
		        result="DRAGON";
		    else
		    {
		        if(dtoc>stoc)
		            result="DRAGON";
		        else if(stoc>dtoc)
		            result="SLOTH";
		        else
		            result="TIE";
		    }
		}
		System.out.println(result);
		 
		 
		    
	}

	}
}
```
