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
- [5️⃣ Operators in Java](#operators-in-java)
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
