# Bear and Candies 123

Read problems statements in Mandarin Chinese, Russian and Vietnamese as well.

Bears love candies and games involving eating them. Limak and Bob play the following game. Limak eats 1 candy, then Bob eats 2 candies, then Limak eats 3 candies, then Bob eats 4 candies, and so on. Once someone can't eat what he is supposed to eat, he loses.

Limak can eat at most A candies in total (otherwise he would become sick), while Bob can eat at most B candies in total. Who will win the game? Print "Limak" or "Bob" accordingly. Input

The first line of the input contains an integer T denoting the number of test cases. The description of T test cases follows.

The only line of each test case contains two integers A and B denoting the maximum possible number of candies Limak can eat and the maximum possible number of candies Bob can eat respectively. Output

For each test case, output a single line containing one string — the name of the winner ("Limak" or "Bob" without the quotes).

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
		    int a=in.nextInt();
		    int b=in.nextInt();
		    int i=1;
		    String winner;
		    while(true)
		    {
		        if((i*i)>a)
		        {
		            winner="Bob";
		            break;
		        }
		        if(i*(i+1)>b)
		        {   
		            winner="Limak";
		            break;
		        }
		      i=i+1;
		    }
		    System.out.println(winner);
		    
		    
		}

	}
}
```
