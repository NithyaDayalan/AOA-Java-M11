# EX 1B Power of 2
## AIM:
To write a Java program to for given constraints.Given an integer n, return true if it is a power of two. Otherwise, return false.

An integer n is a power of two, if there exists an integer x such that n == 2x.

## Algorithm:
1. Read the integer n from the user.
2. Check if n is less than or equal to 0; if yes, return false.
3. Compute n & (n - 1).
4. If the result is 0, then n is a power of two.
5. Print true or false accordingly.

## Program:
```
Developed by: NITHYA D
Register Number: 212223240110
```
```
import java.util.Scanner;

public class Solution {

    public boolean isPowerOfTwo(int n) {
        if (n <= 0) return false;
        return (n & (n - 1)) == 0;
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        Solution sol = new Solution();
        int n = scanner.nextInt();

        boolean result = sol.isPowerOfTwo(n);
        System.out.println(result);

        scanner.close();
    }
}
```
## Output:
<img width="419" height="207" alt="image" src="https://github.com/user-attachments/assets/6b005b6e-77cb-41b6-8d38-41f8fe6616cc" />

## Result:
The program successfully implemented and the expected output is verified.
