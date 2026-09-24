# Ex5 Count Inversions in an Array
## DATE: 11/08/2026
## AIM:
To write a Java program  to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j

## Algorithm

1. Start the program.
2. Read the number of elements and store them in an array.
3. Compare each element with all elements after it.
4. If arr[i] > arr[j] and i < j, increment the inversion count.
5. Display the total number of inversions and stop the program.

## Program:
```
/*
Program to count the number of inversions in an array.
Developed by: HEMALISHA T
RegisterNumber: 212225040123
*/

import java.util.Scanner;

class CountInversions {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter number of elements: ");
        int n = sc.nextInt();

        int arr[] = new int[n];

        System.out.println("Enter array elements:");
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        int count = 0;

        for (int i = 0; i < n - 1; i++) {
            for (int j = i + 1; j < n; j++) {
                if (arr[i] > arr[j]) {
                    count++;
                }
            }
        }

        System.out.println("Number of inversions: " + count);

        sc.close();
    }
}
```

## Output:

<img width="478" height="337" alt="image" src="https://github.com/user-attachments/assets/f9d5cc08-805a-4df3-b9fe-3fbfdc6d7a57" />



## Result:
Thus the Java program to to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < jis implemented successfully.
