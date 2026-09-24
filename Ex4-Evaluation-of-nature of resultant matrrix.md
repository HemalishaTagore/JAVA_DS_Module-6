# Ex4 You are given a Java program that performs matrix addition. If Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension, what will be the nature (even/odd/mixed) of the resulting matrix?
## DATE:11/08/2026
## AIM:
To write a java function to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix.

## Algorithm
1. Start the program.
2. Read the elements of Matrix A and Matrix B of the same dimension.
3. Add the corresponding elements of Matrix A and Matrix B.
4. Check the nature of each element in the resultant matrix.
5. Display the resultant matrix and its nature, then stop the program.

## Program:
```
/*
Program to find the nature of resultant matrix.
Developed by: HEMALISHA T
RegisterNumber: 212225040123
*/

import java.util.Scanner;

class MatrixAddition {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter number of rows: ");
        int r = sc.nextInt();

        System.out.print("Enter number of columns: ");
        int c = sc.nextInt();

        int A[][] = new int[r][c];
        int B[][] = new int[r][c];
        int C[][] = new int[r][c];

        System.out.println("Enter Matrix A (odd numbers):");
        for (int i = 0; i < r; i++) {
            for (int j = 0; j < c; j++) {
                A[i][j] = sc.nextInt();
            }
        }

        System.out.println("Enter Matrix B (even numbers):");
        for (int i = 0; i < r; i++) {
            for (int j = 0; j < c; j++) {
                B[i][j] = sc.nextInt();
            }
        }

        boolean allEven = true;

        System.out.println("Resultant Matrix:");
        for (int i = 0; i < r; i++) {
            for (int j = 0; j < c; j++) {
                C[i][j] = A[i][j] + B[i][j];
                System.out.print(C[i][j] + " ");

                if (C[i][j] % 2 != 0)
                    allEven = false;
            }
            System.out.println();
        }

        if (allEven)
            System.out.println("Nature of resultant matrix: EVEN");
        else
            System.out.println("Nature of resultant matrix: MIXED");

        sc.close();
    }
}
```

## Output:

<img width="662" height="905" alt="image" src="https://github.com/user-attachments/assets/e3bbe239-81ba-4f7f-950a-e03f8b7a6b73" />



## Result:
Thus, the java program to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix is implemented successfully.
