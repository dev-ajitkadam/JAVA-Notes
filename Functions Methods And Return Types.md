# Java Functions, Methods, and Return Types - Notes

## Basic Structure of a Method
A method in Java consists of:
1. **Access Specifier**: Defines visibility (e.g., `public`, `private`).
2. **Modifier**: Alters method behavior (optional; e.g., `static`, `final`).
3. **Return Type**: Type of value returned (e.g., `int`, `void`).
4. **Method Name**: Unique name identifying the method.
5. **Parameter List**: Input parameters (optional).
6. **Method Body**: Code block that defines the task.

## Types of Methods
Built-in Methods: Predefined by Java (e.g., System.out.println()).
User-defined Methods: Created by the programmer.
User-defined Methods
1. Method with Return Type
A method can return a value; the return type specifies its type.

### Example:
```java


java
Copy code
public int add(int a, int b) {
    return a + b;
}

2. Method with Parameters
Methods can take parameters as inputs.

java
Copy code
public void greet(String name) {
    System.out.println("Hello, " + name);
}
3. Method with Modifiers
Modifiers like static and final change method behavior.

Static Method

java
Copy code
public static void displayMessage() {
    System.out.println("This is a static method.");
}
Final Method

java
Copy code
public final void showMessage() {
    System.out.println("This method cannot be overridden.");
}
Example Combining All Concepts
java
Copy code
public class Example {
    // Simple method
    public void printHello() {
        System.out.println("Hello, World!");
    }

    // Method with return type
    public int add(int a, int b) {
        return a + b;
    }

    // Method with parameters
    public void greet(String name) {
        System.out.println("Hello, " + name);
    }

    // Static method
    public static void displayMessage() {
        System.out.println("This is a static method.");
    }

    // Final method
    public final void showMessage() {
        System.out.println("This method cannot be overridden.");
    }

    public static void main(String[] args) {
        Example example = new Example();
        example.printHello();
        System.out.println("Sum: " + example.add(10, 20));
        example.greet("John");
        Example.displayMessage();
        example.showMessage();
    }
}
Explanation:
printHello(): Simple method.
add(int a, int b): Method with return type.
greet(String name): Method with parameters.
displayMessage(): Static method.
showMessage(): Final method.
