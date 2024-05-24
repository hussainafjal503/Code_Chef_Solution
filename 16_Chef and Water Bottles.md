# Chef and Water Bottles

Chef has NN empty bottles where each bottle has a capacity of XX litres.
There is a water tank in Chefland having KK litres of water. Chef wants to fill the empty bottles using the water in the tank.

Assuming that Chef does not spill any water while filling the bottles, find out the maximum number of bottles Chef can fill completely.

Input Format:-

    First line will contain TT, number of test cases. Then the test cases follow.
    Each test case contains of a single line of input, three integers N,X,N,X, and KK.

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
            int total=in.nextInt();
            int water_need=in.nextInt();
            int tank_capacity=in.nextInt();
            if(water_need>tank_capacity)
                System.out.println(0);
            else if(water_need*total<=tank_capacity)
                System.out.println(total);
            else
                System.out.println(tank_capacity/water_need);
                
            
        }
	}
}
```
