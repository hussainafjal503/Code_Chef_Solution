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
	        int x=in.nextInt();
	        int y=in.nextInt();
	        int count=0;
	        if(x==y)
	            System.out.println(0);
	       else
	       {
	           while(y>x)
	           {
	               x=x+8;
	               count+=1;
	               if(x>=y)
	                    break;
	           }
	           System.out.println(count);
	       }
	    }

	}
}
```
