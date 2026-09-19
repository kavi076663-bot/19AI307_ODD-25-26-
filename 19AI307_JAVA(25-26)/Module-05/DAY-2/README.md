# Ex.No:5(B) SERIALIZATION AND DESERIALIZATION 

## QUESTION:


## AIM:


## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	





## PROGRAM:
 ```
/*
Program to implement a Serialization and Deserialization using Java
Developed by: kaviarasu v
RegisterNumber:  212225230132
*/
```

## SOURCE CODE:

```
import java.io.*;
import java.util.Scanner;

class WriterThread extends Thread {
    private PipedOutputStream pos;

    WriterThread(PipedOutputStream pos) {
        this.pos = pos;
    }

    public void run() {
        try {
            Scanner sc = new Scanner(System.in);
            String message = sc.nextLine();
            pos.write(message.getBytes());
            pos.close();
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}

class ReaderThread extends Thread {
    private PipedInputStream pis;

    ReaderThread(PipedInputStream pis) {
        this.pis = pis;
    }

    public void run() {
        try {
            byte[] buffer = new byte[1000];
            int len = pis.read(buffer);
            String received = new String(buffer, 0, len);
            System.out.println("ReaderThread received: " + received);
            pis.close();
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}

class Sourcecode {
    public static void main(String[] args) throws IOException {
        PipedOutputStream pos = new PipedOutputStream();
        PipedInputStream pis = new PipedInputStream(pos);

        WriterThread writer = new WriterThread(pos);
        ReaderThread reader = new ReaderThread(pis);

        writer.start();
        reader.start();
    }
}
```





## OUTPUT:

<img width="918" height="238" alt="image" src="https://github.com/user-attachments/assets/771e9a4a-580c-4d9f-affe-2ddf622a2247" />


## RESULT:
