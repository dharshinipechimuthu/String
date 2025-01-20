# String

import java.util.Scanner;

public class StringOperations {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the first string: ");
        String str1 = scanner.nextLine();       
        System.out.print("Enter the second string: ");
        String str2 = scanner.nextLine();
        System.out.println("\nLength of first string: " + str1.length());
        System.out.println("Length of second string: " + str2.length());
        String concatenatedString = str1 + " " + str2;        System.out.println("\nConcatenated String: " + concatenatedString);
        if (str1.equals(str2)) {
            System.out.println("\nThe strings are equal.");
        } else {
            System.out.println("\nThe strings are not equal.");
        }
        if (str1.contains(str2)) {
            System.out.println("\nThe first string contains the second string.");
        } else {
            System.out.println("\nThe first string does not contain the second string.");
        }
        if (str1.length() > 5) {
            System.out.println("\nSubstring of first string (0 to 5): " + str1.substring(0, 5));
        } else {
            System.out.println("\nThe first string is too short for a substring operation.");
        }
        System.out.println("\nFirst string in uppercase: " + str1.toUpperCase());
        System.out.println("Second string in uppercase: " + str2.toUpperCase());
        scanner.close();
    }
}
input:
Enter the first string: HelloWorld
Enter the second string: World

output:

Length of first string: 10
Length of second string: 5

Concatenated String: HelloWorld World

The strings are not equal.

The first string contains the second string.

Substring of first string (0 to 5): Hello

First string in uppercase: HELLOWORLD
Second string in uppercase: WORLD
 
