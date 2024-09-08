# CodeChef Streak

CodeChef offers a feature called streak count. A streak is maintained if you solve at least one problem daily.

Om and Addy actively maintain their streaks on CodeChef. Over a span of NN consecutive days, you have observed the count of problems solved by each of them.

Your task is to determine the maximum streak achieved by Om and Addy and find who had the longer maximum streak. Input Format

The first line of input will contain a single integer TT, denoting the number of test cases.
Each test case consists of multiple lines of input.
    The first line of each test case contains an integer NN — the number of days.
    The second line of each test case contains NN space-separated integers, the ithith of which is AiAi​, representing the problems solved by Om on the ithith day.
    The third line of each test case contains NN space-separated integers, the ithith of which is BiBi​, representing the problems solved by Addy on the ithith day.

Output Format

For each test case, output:

OM, if Om has longer maximum streak than Addy;
ADDY, if Addy has longer maximum streak than Om;
DRAW, if both have equal maximum streak.

You may print each character in uppercase or lowercase. For example, OM, om, Om, and oM, are all considered the same.

# Java
```java
java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int t = scanner.nextInt();

        while (t-- > 0) {
            int n = scanner.nextInt();
            int[] om = new int[n];
            int[] adday = new int[n];
            
            int count=0,omstrike=0;
            for (int i = 0; i < n; i++) {
                om[i] = scanner.nextInt();
                if(om[i]==0)
                    count=0;
                else
                    count++;
                    
                if(count>omstrike)
                    omstrike=count;
            }

            count=0;
            int addaystrike=0;
            for (int j = 0; j < n; j++) {
                adday[j] = scanner.nextInt();
                if(adday[j]==0)
                    count=0;
                else
                    count++;
                    
                if(count>addaystrike)
                    addaystrike=count;
            }
            
          
        
             if(omstrike==addaystrike){
                System.out.println("Draw");
            }
            else if(omstrike>addaystrike){
                System.out.println("Om");
            }
            else{
                System.out.println("Addy");
            }
        
        }
        
    }
}
```
