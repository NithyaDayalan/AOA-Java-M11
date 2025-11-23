# EX 1A Print All Numbers 
## AIM:
To Write a Java program that takes an integer input N from the user and prints all the numbers from 1 to N, separated by spaces, on a single line..

## Algorithm:
1. Read the input value N from the user.
2. Check if N is less than or equal to 0.
3. If true, display "Invalid input".
4. If false, start a loop from 1 to N.
5. Print each number in the loop separated by spaces. 

## Program:
```
Developed by: NITHYA D
Register Number: 212223240110
```
```
import java.util.Scanner;
public class PrintNumbers {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int N = scanner.nextInt();
        if (N <= 0) {
            System.out.println("Invalid input. N must be greater than 0.");
        } else {
            for (int i = 1; i <= N; i++) {
                System.out.print(i + " ");
            }
        }
        scanner.close();
    }
}

```
## Output:
<img width="437" height="164" alt="image" src="https://github.com/user-attachments/assets/80a52f54-bebd-490c-b262-7eccab179274" />

## Result:
The program successfully print all the numbers from 1 to N. 
