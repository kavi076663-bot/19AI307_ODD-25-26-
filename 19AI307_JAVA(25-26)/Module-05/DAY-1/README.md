# Ex.No:5(A) INPUTSTREAMREADER 

## QUESTION:


## AIM:


## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	





## PROGRAM:
 ```
/*
Program to implement a InputStreamReader using Java
Developed by: v.kaviarasu
RegisterNumber:  212225230132
*/
```

## SOURCE CODE:
```
import java.io.FileWriter;
import java.io.IOException;
import java.util.Scanner;

class Sourcecode {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String filename = sc.nextLine();
        String content = sc.nextLine();

        try {
            FileWriter fw = new FileWriter(filename);
            fw.write(content);
            fw.close();
            System.out.println("File written successfully.");
        } catch (IOException e) {
            System.out.println("An error occurred.");
        }
    }
}
```






## OUTPUT:

<img width="913" height="316" alt="image" src="https://github.com/user-attachments/assets/bb7b70c0-08ae-4541-b908-e39d002aaabd" />


## RESULT:
