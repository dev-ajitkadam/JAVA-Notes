# Exception & Exception Handling - Short Notes

## What is an Exception?
An exception is an event that disrupts the normal flow of a program's execution. It represents an error or unexpected event during runtime.

## What is Exception Handling?
Exception handling allows the program to handle runtime errors gracefully, preventing the program from crashing. Keywords used for exception handling in Java are: `try`, `catch`, `finally`, `throw`, and `throws`.

## Types of Exceptions
1. **Checked Exceptions**: 
   - Checked at compile-time.
   - Must be handled or declared using `throws`.
   - Examples: `IOException`, `SQLException`.

2. **Unchecked Exceptions**: 
   - Occur at runtime and are not checked at compile-time.
   - Commonly programming errors.
   - Examples: `ArrayIndexOutOfBoundsException`, `NullPointerException`.

3. **Errors**: 
   - Serious issues that are usually beyond the control of the program.
   - Not typically handled in code.
   - Examples: `OutOfMemoryError`, `StackOverflowError`.

## Code Examples

### Checked Exception Example:
```java
import java.io.*;
public class CheckedExceptionExample {
    public static void main(String[] args) {
        try {
            FileReader file = new FileReader("test.txt");
        } catch (FileNotFoundException e) {
            System.out.println("File not found.");
        }
    }
}

Unchecked Exception Example:
java
Copy code
public class UncheckedExceptionExample {
    public static void main(String[] args) {
        try {
            int[] numbers = {1, 2, 3};
            System.out.println(numbers[10]);
        } catch (ArrayIndexOutOfBoundsException e) {
            System.out.println("Array index out of bounds.");
        }
    }
}
Error Example:
java
Copy code
public class ErrorExample {
    public static void main(String[] args) {
        try {
            recurse();
        } catch (StackOverflowError e) {
            System.out.println("StackOverflowError.");
        }
    }

    public static void recurse() {
        recurse();
    }
}
Summary
Exception: An event disrupting normal program flow.
Exception Handling: Managing runtime errors with try, catch, finally, throw, and throws.
Types:
Checked: Declared or handled at compile-time.
Unchecked: Runtime errors.
Errors: Serious issues, not handled in code.
