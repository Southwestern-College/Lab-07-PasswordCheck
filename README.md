# Lab: Password Check

## Program Description
Write a Java method to check whether a string is a valid password.

### Password Rules:
- A password must have **at least 8 characters** and **at most 32 characters**.
- A password consists of **only letters, digits**, and the following **special characters**:
  - `! " # $ % & ' ( ) * + , - . /`
  - *(Note: These characters have consecutive ASCII values.)*
- A valid password must contain:
  - At least one lowercase letter
  - At least one uppercase letter
  - At least one digit
  - At least one special character
  - *No characters other than those mentioned above*
  - If a password does not meet these conditions, it is **not valid**.

## Program Specifications
Consider the following class:

```java
import java.util.Scanner;

public class PasswordCheck {

  public static void main(String[] args) {
      // Create a Scanner object to receive user input from keyboard
      Scanner input = new Scanner(System.in);

      String password;
      
      // Prompt user for a password until they enter a valid password
      do {
          System.out.println("Please enter a password:");
          password = input.nextLine();
      } while (!isValidPassword(password));

      System.out.println("Success");
  } 

  public static boolean isValidPassword(String password) { 
      // Complete this code
  }

  public static boolean isUpperCase(char ch) {
      // Complete this code
  }

  public static boolean isLowerCase(char ch) {
      // Complete this code
  }

  public static boolean isDigit(char ch) {
      // Complete this code
  }

  public static boolean isSpecialCharacter(char ch) {
      // Complete this code
  }
}
```

Complete the following methods:
- `isUpperCase(char ch)`: Returns true if the argument is an uppercase character, otherwise returns false.
- `isLowerCase(char ch)`: Returns true if the argument is a lowercase character, otherwise returns false.
- `isDigit(char ch)`: Returns true if the argument is a digit, otherwise returns false.
- `isSpecialCharacter(char ch)`: Returns true if the argument is a valid special character, otherwise returns false.
- `isValidPassword(String password)`: Returns true if the argument is a valid password, otherwise returns false.
  - `isValidPassword` must print an error message for each password rule that has been violated.

## CODING STANDARDS
- Adhere to the program specifications.
- Use meaningful variable names.
- Remove any auto-generated comments.
- Use [JavaDoc](https://en.wikipedia.org/wiki/Javadoc) to document your code.
- Include a program description and attribute yourself using the `@author` tag.
- Your output should be user-friendly.
