# Ex2 Count how many times a number appears in an array recursively.
## DATE: 14/08/2026
## AIM:
To write a Java program to Count how many times a number appears in an array recursively.
## Algorithm
1. Start the program.
2. Read the number of elements and store them in an array.
3. Read the number to be searched.
4. Use a recursive method to count how many times the number appears in the array.
5. Display the count and stop the program.

## Program:
```
/*
Program to count how many times a number appears in an array recursively.
Developed by: HEMALISHA T
RegisterNumber: 212225040123
*/

import java.util.Scanner;

class CountRecursive {

    static int countNumber(int arr[], int n, int num) {
        if (n == 0)
            return 0;

        if (arr[n - 1] == num)
            return 1 + countNumber(arr, n - 1, num);
        else
            return countNumber(arr, n - 1, num);
    }

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter number of elements: ");
        int n = sc.nextInt();

        int arr[] = new int[n];

        System.out.println("Enter array elements:");
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        System.out.print("Enter number to count: ");
        int num = sc.nextInt();

        int count = countNumber(arr, n, num);

        System.out.println("Number of times " + num + " appears: " + count);

        sc.close();
    }
}
```

## Output:

<img width="283" height="262" alt="image" src="https://github.com/user-attachments/assets/97f60edc-487d-43b0-94fa-160530854d78" />


## Result:
Thus, the Java program to Count how many times a number appears in an array recursively is implemented successfully.
