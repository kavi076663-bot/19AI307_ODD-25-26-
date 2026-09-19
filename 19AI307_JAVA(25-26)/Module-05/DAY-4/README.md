# Ex.No:5(D) THREAD PRIORITY

## QUESTION:


## AIM:


## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	





## PROGRAM:
 ```
/*
Program to implement a Thread Priority Concept using Java
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

        String threadName = sc.nextLine();

        Thread t = Thread.currentThread();

        t.setName(threadName);
        t.setPriority(2);

        System.out.println("Priority of Thread: " + t.getPriority());
        System.out.println("Name of Thread: " + t.getName());
        System.out.println(t);
    }
}
```






## OUTPUT:
<img width="816" height="183" alt="image" src="https://github.com/user-attachments/assets/3331c131-9c10-4e7a-864f-e916d6b375f8" />




## RESULT:
