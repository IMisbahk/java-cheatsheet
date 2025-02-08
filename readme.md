# **Java Cheatsheet**  

Welcome to the **Java Cheatsheet**! 🚀 This is a **comprehensive, one-stop reference** for Java, covering everything from **fundamentals to advanced topics** in a clean and structured way.  

## **📌 What You'll Find Here**  
- **Clear explanations** of Java concepts.  
- **Tables for quick reference** to syntax and key functions.  
- **Copy-paste-ready code snippets** to test and modify instantly.  
- **A structured flow** from beginner-friendly topics to advanced Java features.  

## **💡 Why This Cheatsheet?**  
- **Everything in one place** – No need to jump between docs.  
- **Quick and practical** – Get straight to the point with ready-to-use examples.  
- **Perfect for revision** – Search, copy, and implement easily.  

---


## **📖 Table of Contents**

### 🟢 **Beginner (Class 9)**
- [1️⃣ Introduction to Object-Oriented Programming Concepts](#introduction-to-object-oriented-programming-concepts)
- [2️⃣ Introduction to Java](#introduction-to-java)
- [3️⃣ Elementary Concepts of Objects and Classes](#elementary-concepts-of-objects-and-classes)
- [4️⃣ Values and Data Types](#values-and-data-types)
- [5️⃣ Operators in Java](#Operators-in-java)
- [6️⃣ Input in Java](#input-in-java)
- [7️⃣ Conditional Constructs in Java](#conditional-constructs-in-java)
- [8️⃣ Iterative Constructs in Java](#iterative-constructs-in-java)
- [9️⃣ Nested for Loops](#nested-for-loops)

### 🔵 **Intermediate (Class 10)**
- [🔟 Class as the Basis of All Computation](#class-as-the-basis-of-all-computation)
- [1️⃣1️⃣ User-Defined Methods](#user-defined-methods)
- [1️⃣2️⃣ Constructors](#constructors)
- [1️⃣3️⃣ Library Classes](#library-classes)
- [1️⃣4️⃣ Encapsulation](#encapsulation)
- [1️⃣5️⃣ Arrays](#arrays)
- [1️⃣6️⃣ String Handling](#string-handling)

### 🔴 **Advanced (Class 11)**
- [1️⃣7️⃣ Introduction to Algorithmic Problem Solving Using Java](#introduction-to-algorithmic-problem-solving-using-java)
- [1️⃣8️⃣ Objects](#objects)
- [1️⃣9️⃣ Primitive Values, Wrapper Classes, Types, and Casting](#primitive-values-wrapper-classes-types-and-casting)
- [2️⃣0️⃣ Variables and Expressions](#variables-and-expressions)
- [2️⃣1️⃣ Statements and Scope](#statements-and-scope)
- [2️⃣2️⃣ Methods and Constructors](#methods-and-constructors)
- [2️⃣3️⃣ Arrays and Strings](#arrays-and-strings)
- [2️⃣4️⃣ Basic Input/Output and Data File Handling](#basic-inputoutput-and-data-file-handling)
- [2️⃣5️⃣ Recursion](#recursion)
- [2️⃣6️⃣ Implementation of Algorithms to Solve Problems](#implementation-of-algorithms-to-solve-problems)
- [2️⃣7️⃣ Packages](#packages)
- [2️⃣8️⃣ Trends in Computing and Ethical Issues](#trends-in-computing-and-ethical-issues)

---

### 1️⃣ Introduction to Object-Oriented Programming (OOP)  

- Java is an **object-oriented** programming language.  
- OOP is based on **objects** (real-world entities) and **classes** (blueprints for objects).  
- Four key principles of OOP:  

  | Principle      | Meaning |
  |--------------|---------|
  | **Encapsulation** | Wrapping data and methods together to protect information. |
  | **Inheritance** | One class can inherit properties from another. |
  | **Polymorphism** | Methods can behave differently based on the object calling them. |
  | **Abstraction** | Hides unnecessary details and shows only essential features. |

**Example:**  
```java
class Car {
    String color;
    void startEngine() {
        System.out.println("Engine started.");
    }
}
```

---

### 2️⃣ Introduction to Java  

- Java is **platform-independent** (Write Once, Run Anywhere).  
- **Compiling a Java program:**  

  ```java
  // Source Code (Hello.java)
  class Hello {
      public static void main(String[] args) {
          System.out.println("Hello, Java!");
      }
  }
  ```

  - `javac Hello.java` → Compiles the program.  
  - `java Hello` → Runs the compiled program.  

---

### 3️⃣ Objects and Classes  

- **Class**: A blueprint that defines attributes and methods.  
- **Object**: An instance of a class with actual values.  

**Example:**  
```java
class Car {
    String color;
    void startEngine() {
        System.out.println("Engine started.");
    }
}

public class Main {
    public static void main(String[] args) {
        Car myCar = new Car();
        myCar.color = "Red";
        myCar.startEngine(); // Output: Engine started.
    }
}
```

---

### 4️⃣ Values and Data Types  

- Java has different **data types** to store different kinds of values.  
- Data types are categorized into **primitive** and **non-primitive**.  

#### **Primitive Data Types**  

| Data Type  | Size      | Example |
|------------|----------|---------|
| `byte`     | 1 byte   | `byte b = 100;` |
| `short`    | 2 bytes  | `short s = 32000;` |
| `int`      | 4 bytes  | `int num = 10;` |
| `long`     | 8 bytes  | `long bigNum = 100000L;` |
| `float`    | 4 bytes  | `float pi = 3.14f;` |
| `double`   | 8 bytes  | `double precise = 3.14159;` |
| `char`     | 2 bytes  | `char letter = 'A';` |
| `boolean`  | 1 bit    | `boolean isJavaFun = true;` |

#### **Non-Primitive Data Types**  
- Strings, Arrays, Classes, and Interfaces are non-primitive types.  
- Example:  
  ```java
  String message = "Hello, Java!";
  ```

---

### 5️⃣ Operators in Java  

- Operators perform operations on variables and values.  
- Java has different categories of operators:  

| Operator Type      | Uses |
|--------------------|-----------------------------|
| **Arithmetic**     | `+`, `-`, `*`, `/`, `%`  |
| **Relational**     | `==`, `!=`, `>`, `<`, `>=`, `<=` |
| **Logical**        | `&&`, `||`, `!` |
| **Bitwise**        | `&`, `|`, `^`, `~`, `<<`, `>>` |
| **Assignment**     | `=`, `+=`, `-=`, `*=`, `/=`, `%=` |
| **Unary**          | `+`, `-`, `++`, `--` |
| **Ternary**        | `condition ? trueValue : falseValue` |

**Example:**  
```java
int a = 10, b = 5;
System.out.println(a + b); // Output: 15
System.out.println(a > b); // Output: true
System.out.println(a == 10 && b < 10); // Output: true
```

---
### 6️⃣ Input and Output in Java  

- Java provides the `Scanner` class for user input.  
- `System.out.println()` is used to display output.  

#### **Taking Input Using Scanner**  
```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        System.out.print("Enter your name: ");
        String name = sc.nextLine();  // Takes string input
        
        System.out.print("Enter your age: ");
        int age = sc.nextInt();  // Takes integer input
        
        System.out.println("Hello, " + name + "! You are " + age + " years old.");
    }
}
```

#### **Printing Output**
```java
System.out.println("Hello, Java!"); // Prints with a new line
System.out.print("Hello, "); // Prints without a new line
System.out.printf("Pi value: %.2f", 3.14159); // Formatted output
```

---

### 7️⃣ Control Flow Statements  

Java provides control statements to **change the flow of execution**.  

#### **Conditional Statements**  

- **If Statement**  
  ```java
  if (condition) {
      // Code executes if condition is true
  }
  ```

- **If-Else Statement**  
  ```java
  if (condition) {
      // Code executes if condition is true
  } else {
      // Code executes if condition is false
  }
  ```

- **Else-If Ladder**  
  ```java
  if (condition1) {
      // Executes if condition1 is true
  } else if (condition2) {
      // Executes if condition2 is true
  } else {
      // Executes if none of the conditions are true
  }
  ```

- **Switch Statement**  
  ```java
  int day = 3;
  switch (day) {
      case 1:
          System.out.println("Monday");
          break;
      case 2:
          System.out.println("Tuesday");
          break;
      default:
          System.out.println("Other day");
  }
  ```

---

### 8️⃣ Looping Statements  

Loops help in **executing a block of code multiple times**.  

#### **While Loop**  
Executes while the condition is **true**.  
```java
int i = 1;
while (i <= 5) {
    System.out.println(i);
    i++;
}
```

#### **Do-While Loop**  
Executes at least **once**, then checks the condition.  
```java
int i = 1;
do {
    System.out.println(i);
    i++;
} while (i <= 5);
```

#### **For Loop**  
Used when the number of iterations is **fixed**.  
```java
for (int i = 1; i <= 5; i++) {
    System.out.println(i);
}
```

#### **For-Each Loop**  
Used to **iterate over arrays or collections**.  
```java
int[] numbers = {1, 2, 3, 4, 5};
for (int num : numbers) {
    System.out.println(num);
}
```

---

### 9️⃣ Jump Statements  

- **Break Statement** → Exits the loop immediately.  
  ```java
  for (int i = 1; i <= 5; i++) {
      if (i == 3) {
          break;
      }
      System.out.println(i); // Output: 1 2
  }
  ```

- **Continue Statement** → Skips the current iteration and proceeds to the next.  
  ```java
  for (int i = 1; i <= 5; i++) {
      if (i == 3) {
          continue;
      }
      System.out.println(i); // Output: 1 2 4 5
  }
  ```
---
## 🔵 Intermediate (Class 10)  

### 🔟 Class as the Basis of All Computation  

- **A class is a blueprint** for creating objects in Java.  
- It contains **fields (variables)** and **methods (functions)**.  

#### **Example of a Class and Object**  
```java
class Car {
    String model = "Tesla"; // Instance variable

    void displayModel() { // Method
        System.out.println("Car Model: " + model);
    }

    public static void main(String[] args) {
        Car myCar = new Car(); // Object creation
        myCar.displayModel();  // Calling the method
    }
}
```

---

### 1️⃣1️⃣ User-Defined Methods  

- **Methods** allow us to break a program into smaller, reusable parts.  
- There are **two types** of methods:  
  - **Methods that return a value**  
  - **Methods that do not return a value**  

#### **Method Without Return Type**  
```java
public class Main {
    static void greet() {
        System.out.println("Hello, Java!");
    }

    public static void main(String[] args) {
        greet(); // Calling the method
    }
}
```

#### **Method With Return Type**  
```java
public class Main {
    static int add(int a, int b) {
        return a + b;
    }

    public static void main(String[] args) {
        int sum = add(5, 10);
        System.out.println("Sum: " + sum);
    }
}
```

---
### 1️⃣2️⃣ Constructors  

- A **constructor** is a special method that initializes objects.  
- It has **the same name as the class** and **no return type**.  

#### **Types of Constructors**  
| Constructor Type   | Description |
|-------------------|-------------|
| **Default Constructor** | No parameters, assigns default values. |
| **Parameterized Constructor** | Takes arguments to initialize values. |

#### **Example: Default Constructor**  
```java
public class Car {
    Car() { // Constructor
        System.out.println("Car object created!");
    }

    public static void main(String[] args) {
        Car myCar = new Car(); // Calls the constructor
    }
}
```

#### **Example: Parameterized Constructor**  
```java
public class Car {
    String model;

    // Constructor with parameter
    Car(String carModel) {
        model = carModel;
    }

    public static void main(String[] args) {
        Car myCar = new Car("Tesla");
        System.out.println("Car Model: " + myCar.model);
    }
}
```

---

### 1️⃣3️⃣ Library Classes  

- Java provides **built-in classes** for various functionalities.  
- Common library classes:  
  - **Math** (mathematical operations)  
  - **String** (string manipulations)  
  - **Scanner** (user input handling)  

#### **Using Math Library**  
```java
public class Main {
    public static void main(String[] args) {
        System.out.println(Math.sqrt(25));  // 5.0
        System.out.println(Math.pow(2, 3)); // 8.0
    }
}
```

#### **Using Scanner Library**  
```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter your name: ");
        String name = sc.nextLine();
        System.out.println("Hello, " + name);
        sc.close();
    }
}
```

---

### 1️⃣4️⃣ Encapsulation  

- **Encapsulation** is the practice of **hiding data** within a class and controlling access through methods.  
- We use **private variables** and **public getter/setter methods**.  

#### **Example of Encapsulation**  
```java
public class Person {
    private String name; // Private variable

    // Setter method
    public void setName(String newName) {
        name = newName;
    }

    // Getter method
    public String getName() {
        return name;
    }

    public static void main(String[] args) {
        Person p = new Person();
        p.setName("Alice");
        System.out.println("Name: " + p.getName());
    }
}
```

---

### 🔟 Arrays in Java  

- An **array** is a collection of elements of the **same data type**.  
- Java arrays have **fixed size** once declared.  

#### **Declaring and Initializing an Array**  
```java
int[] numbers = {10, 20, 30, 40, 50};
String[] names = new String[3]; // Empty array of size 3
names[0] = "Alice"; // Assigning values
```

#### **Accessing and Modifying Array Elements**  
```java
System.out.println(numbers[0]); // Output: 10
numbers[2] = 99; // Modifying an element
```

#### **Looping Through an Array**  
```java
for (int i = 0; i < numbers.length; i++) {
    System.out.println(numbers[i]); // Using a for loop
}

for (int num : numbers) {
    System.out.println(num); // Using a for-each loop
}
```


---

### 1️⃣6️⃣ String Handling  

- **Strings** are sequences of characters stored in **String objects**.  
- Strings are **immutable**, meaning they cannot be changed after creation.  

#### **Declaring Strings**  
```java
String s1 = "Hello";
String s2 = new String("Java");
```

#### **Common String Methods**  
| Method | Description |
|--------|------------|
| `length()` | Returns string length |
| `charAt(index)` | Returns character at index |
| `substring(start, end)` | Extracts substring |
| `toUpperCase()` | Converts to uppercase |
| `toLowerCase()` | Converts to lowercase |
| `concat(str)` | Joins two strings |

#### **Example: String Methods**  
```java
public class Main {
    public static void main(String[] args) {
        String str = "Hello, Java";
        System.out.println(str.length());       // 11
        System.out.println(str.charAt(1));      // e
        System.out.println(str.substring(0, 5)); // Hello
        System.out.println(str.toUpperCase());  // HELLO, JAVA
    }
}
```

---

[🔼 Back to Top](#java-fundamentals-cheatsheet) | [🔷 Next: Advanced](#advanced-class-11)  
