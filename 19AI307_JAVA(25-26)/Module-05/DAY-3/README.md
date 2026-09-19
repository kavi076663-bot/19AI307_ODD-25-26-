# Ex.No:5(C)  FILE HANDLING USING JAVA
## QUESTION:


## AIM:


## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	





## PROGRAM:
 ```
/*
Program to implement a File Handling using Java
Developed by: kaviarasu v
RegisterNumber:  212225230132
*/
```

## SOURCE CODE:

```
import java.util.*;

class Sourcecode {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        ArrayList<String> matchingLines = new ArrayList<>();

        while (true) {
            String line = sc.nextLine();
            if (line.equals("exit"))
                break;

            if (line.contains("Java"))
                matchingLines.add(line);
        }

        System.out.println("Lines containing the word 'Java':");
        for (String s : matchingLines) {
            System.out.println(s);
        }
    }
}
```





## OUTPUT:
<img width="1123" height="324" alt="image" src="https://github.com/user-attachments/assets/1a24212e-fe0f-4314-8dd0-cbe678be8b5e" />



## RESULT:
