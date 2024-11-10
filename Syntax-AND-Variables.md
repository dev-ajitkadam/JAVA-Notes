
# Java Syntax and Variables

## Java Syntax and Structure
- **Keywords**: Reserved words with specific functions (e.g., `class`, `public`, `static`, `void`, `if`, `else`).

- **Comments**: Improve readability and are ignored by the compiler.
  - **Single-line**: `// comment`
  - **Multi-line**: `/* comment */`
  - **Documentation**: `/** comment */`

## Main Method
- Entry point of a Java program with a specific signature:
  ```java
  public static void main(String[] args) {
      // Code here
  }
  ```
  - **public**: Accessible from anywhere.
  - **static**: Can be called without creating an instance.
  - **void**: No return value.
  - **String[] args**: Accepts a string array as an argument.

## Class and Object
- **Class**: A blueprint for creating objects, bundling data and methods.
- **Object**: An instance of a class, created with `new`.

  ```java
  public class Car {
      String color;
      String model;
      void drive() { System.out.println("The car is driving."); }
  }
  ```

## Literals
- Fixed values assigned to variables or used in expressions.
  - **Integer**: `int x = 100;`
  - **Float**: `double y = 10.5;`
  - **Char**: `char z = 'A';`
  - **String**: `String s = "Hello";`
  - **Boolean**: `boolean b = true;`

## Methods
- Blocks of code that perform a task.
- Can return a value or be `void` if not returning anything.

  ```java
  public class Calculator {
      public int add(int a, int b) { return a + b; }
      public void printMessage() { System.out.println("Hello, World!"); }
  }
  ```

## Variables
- Containers for data, with Java being strongly typed.
- **Identifiers**: Names for elements (variables, methods, etc.), starting with a letter, underscore, or dollar sign, using camelCase for variables and PascalCase for classes.

## Variable Types
1. **Local Variables**: Declared within methods or blocks; no default values.
   ```java
   public void myMethod() { int localVar = 10; }
   ```
2. **Instance Variables**: Declared in a class but outside methods; have default values.
   ```java
   public class MyClass { int instanceVar; }
   ```
   
---

These notes cover the essentials of Java syntax, comments, main method structure, class and object creation, literals, methods, and types of variables.
