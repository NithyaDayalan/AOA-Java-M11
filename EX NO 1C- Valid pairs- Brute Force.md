# EX 1C Valid Pairs using Brute Force Approach
## AIM:
To write a Java program to for given constraints.
Given an integer array nums and an integer k, return the number of pairs (i, j) where i < j such that |nums[i] - nums[j]| == k.

The value of |x| is defined as:

x if x >= 0.
-x if x < 0.

## Algorithm:
1. Read the size of the array and input all elements.
2. Read the value of k.
3. Initialize count to 0.
4. Compare every pair of elements and check if their absolute difference equals k.
5. Increment count for each valid pair and print the final count.  

## Program:
```
Developed by: NITHYA D
Register Number: 212223240110
```
```
import java.util.Scanner;
public class CountPairsWithDifference {
    public static int countKDifference(int[] nums, int k) {
        int count = 0;
        for (int i = 0; i < nums.length; i++) {
            for (int j = i + 1; j < nums.length; j++) {
                if (Math.abs(nums[i] - nums[j]) == k) {
                    count++;
                }
            }
        }
        return count;
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] nums = new int[n];
        for (int i = 0; i < n; i++) {
            nums[i] = sc.nextInt();
        }
        int k = sc.nextInt();
        int result = countKDifference(nums, k);
        System.out.println(result);
        sc.close();
    }
}
```

## Output:
<img width="458" height="296" alt="image" src="https://github.com/user-attachments/assets/5763c0e8-cd7e-4428-af73-f96cf8e01a24" />

## Result:
The program successfully implemented and the expected output is verified.
