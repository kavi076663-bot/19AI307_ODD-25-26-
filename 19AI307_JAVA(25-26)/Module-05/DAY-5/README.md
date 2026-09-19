# Ex.No:5(E) MULTITHREADING -SYNCHRONIZATION

## QUESTION:


## AIM:


## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	





## PROGRAM:
 ```
/*
Program to implement a Synchronization concept using Java
Developed by: kaviarasu v
RegisterNumber:  212225230132
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Sourcecode {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int a = sc.nextInt();
        int b = sc.nextInt();

        Object lock = new Object();

        synchronized (lock) {
            int temp = a;
            a = b;
            b = temp;
        }

        System.out.println("a = " + a);
        System.out.println("b = " + b);
    }
}
```






## OUTPUT:
<img width="415" height="307" alt="image" src="https://github.com/user-attachments/assets/12a852b7-bb4a-4d4d-aba3-8c4db53d33d2" />



## RESULT:
