# EX 1 You’re creating a health monitoring device which stores several sensor readings in an array. To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
## DATE:
## AIM:
To write a JAVA program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.

## Algorithm
1. Start the program.
2. Read the number of sensor readings and store them in an array.
3. Define a recursive method to find the minimum value in the array.
4. Compare the last element with the minimum value returned by the recursive call.
5. Display the minimum sensor reading and stop the program.

## Program:
```
/*
Program to determine the minimum value using recursion
Developed by: HEMALISHA T
RegisterNumber: 212225040123
*/

import java.util.Scanner;

class MinimumRecursive {

    static int findMin(int arr[], int n) {
        if (n == 1)
            return arr[0];

        return Math.min(arr[n - 1], findMin(arr, n - 1));
    }

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter number of sensor readings: ");
        int n = sc.nextInt();

        int arr[] = new int[n];

        System.out.println("Enter sensor readings:");
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        int min = findMin(arr, n);

        System.out.println("Minimum sensor reading: " + min);

        sc.close();
    }
}
```

## Output:
<img width="336" height="208" alt="image" src="https://github.com/user-attachments/assets/589ceab4-107b-424a-9a34-d64321a1eb5f" />



## Result:
Thus the JAVA prograM ti find the minimum value (e.g., lowest heartbeat), implement a recursive method has implemented successfully
