# EX3 Write a program to count the number of digits in an integer.
## DATE: 11/08/2026
## AIM:
To write a C program to implement Tower of Hanoi

## Algorithm
1. Start the program.
2. Read an integer from the user.
3. Divide the number by 10 repeatedly and increment the count.
4. Continue until the number becomes 0.
5. Display the number of digits and stop the program.

## Program:
```
/*
Program to count the number of digits in an integer
Developed by: HEMALISHA T
RegisterNumber: 212225040123
*/

import java.util.Scanner;

class CountDigits {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter an integer: ");
        int num = sc.nextInt();

        int count = 0;
        int n = Math.abs(num);

        if (n == 0) {
            count = 1;
        } else {
            while (n > 0) {
                n = n / 10;
                count++;
            }
        }

        System.out.println("Number of digits: " + count);

        sc.close();
    }
}
```

## Output:
<img width="822" height="353" alt="image" src="https://github.com/user-attachments/assets/0a6a1649-d8f2-424f-b2dd-e5fb8d7ed8bf" />




## Result:
Thus, the Java program to to count the number of digits in an integer is implemented successfully.
