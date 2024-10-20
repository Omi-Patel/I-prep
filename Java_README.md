# Java Interview Preparation Guide

## Table of Contents

1. [Introduction to Java](#introduction-to-java)
2. [Basic Concepts in Java](#basic-concepts-in-java)
   - Variables
   - Data Types
   - Operators
   - Control Flow Statements
3. [Object-Oriented Programming in Java](#object-oriented-programming-oop-in-java)
   - Classes and Objects
   - Constructors
   - Inheritance
   - Polymorphism
   - Abstraction
   - Encapsulation
   - Interfaces
4. [Exception Handling](#exception-handling)
5. [Collections Framework](#collections-framework)
6. [Multithreading](#multithreading)
7. [Java I/O](#java-input-output)
8. [Java 8 Features](#java-8-features)
9. [Common Java Interview Questions and Answers](#common-java-interview-questions-and-answers)

---

## Introduction to Java

Java is a high-level, class-based, object-oriented programming language designed to have as few implementation dependencies as possible. It is widely used due to its platform independence.

- **Platform Independence**: Java programs are compiled into bytecode, which can run on any system equipped with the Java Virtual Machine (JVM).
- **Object-Oriented**: Everything in Java revolves around objects and classes.
- **Multithreading Support**: Java provides built-in support for concurrent programming.

---

## Basic Concepts in Java

### Variables

Variables are containers for storing data values. In Java, you need to declare variables before using them.

```java
int age = 25;
String name = "John";
```

### Data Types

Java has two types of data types:

- **Primitive Data Types**: `int`, `float`, `char`, `boolean`, etc.
- **Reference Data Types**: Objects, arrays, etc.

### Operators

Java supports:

- **Arithmetic Operators**: `+`, `-`, `*`, `/`, `%`
- **Relational Operators**: `==`, `!=`, `>`, `<`, `>=`, `<=`
- **Logical Operators**: `&&`, `||`, `!`

### Control Flow Statements

- **if-else**
- **switch-case**
- **for loop**
- **while loop**
- **do-while loop**

---

## Object-Oriented Programming (OOP) in Java

### Classes and Objects

A **class** is a blueprint from which individual objects are created.

```java
class Car {
   String model;
   int year;
   void drive() {
      System.out.println("Driving the car...");
   }
}
```

### Constructors

A **constructor** initializes an object when it is created.

```java
class Car {
   String model;
   int year;

   // Constructor
   Car(String m, int y) {
      model = m;
      year = y;
   }
}
```

### Inheritance

**Inheritance** allows one class to inherit fields and methods from another class.

```java
class Animal {
   void eat() {
      System.out.println("Eating...");
   }
}

class Dog extends Animal {
   void bark() {
      System.out.println("Barking...");
   }
}
```

### Polymorphism

**Polymorphism** allows one method to have different forms (e.g., method overloading and method overriding).

- **Method Overloading**: Same method name, different parameters.
- **Method Overriding**: A subclass provides its specific implementation of a method.

### Abstraction

**Abstraction** hides internal details and shows only the essential features of an object.

### Encapsulation

**Encapsulation** binds data and methods together and keeps them safe from outside interference.

### Interfaces

An **interface** in Java is a blueprint of a class that contains abstract methods. It is used to achieve abstraction and multiple inheritance.

---

## Exception Handling

Java provides a powerful exception handling mechanism that is used to handle runtime errors, making the code robust and error-free.

```java
try {
    // Code that may throw an exception
} catch (Exception e) {
    // Handle exception
} finally {
    // Code that will always execute
}
```

---

## Collections Framework

Java Collections Framework provides data structures and algorithms that help store and manipulate data.

- **List**: ArrayList, LinkedList
- **Set**: HashSet, TreeSet
- **Map**: HashMap, TreeMap
- **Queue**: PriorityQueue

---

## Multithreading

Java supports **multithreading**, which allows concurrent execution of two or more parts of a program to maximize the utilization of CPU.

```java
class MyThread extends Thread {
   public void run() {
      System.out.println("Thread is running.");
   }
}
```

---

## Java Input/Output

Java I/O provides APIs to handle input and output through data streams, serialization, file handling, etc.

```java
FileReader fr = new FileReader("file.txt");
BufferedReader br = new BufferedReader(fr);
```

---

## Java 8 Features

- **Lambda Expressions**: Provide a clear and concise way to represent one method interface using an expression.
- **Stream API**: A sequence of elements supporting sequential and parallel aggregate operations.
- **Functional Interfaces**: Interfaces with only one abstract method.

---

## Common Java Interview Questions and Answers

### 1. What is the difference between JDK, JRE, and JVM?

- **JDK (Java Development Kit)**: A software development environment for building Java applications.
- **JRE (Java Runtime Environment)**: Provides libraries and other components to run applications written in Java.
- **JVM (Java Virtual Machine)**: Executes Java bytecode and provides an environment for Java programs to run.

### 2. What is the difference between abstraction and encapsulation?

- **Abstraction** hides complexity by showing only the essential features of an object.
- **Encapsulation** wraps data (variables) and code (methods) into a single unit and restricts access to some of the object's components.

### 3. What is method overloading and method overriding?

- **Method Overloading**: Multiple methods with the same name but different parameter lists.
- **Method Overriding**: A subclass provides a specific implementation of a method that is already defined in its superclass.

### 4. What is the difference between an abstract class and an interface?

- **Abstract Class**: Can have abstract and non-abstract methods, and can maintain state.
- **Interface**: Can only have abstract methods (until Java 8), and does not maintain state.

### 5. What is polymorphism and how is it achieved in Java?

**Polymorphism** allows an object to take many forms. It can be achieved through:

- **Method Overloading** (Compile-time polymorphism)
- **Method Overriding** (Runtime polymorphism)

### 6. What are static members in Java?

**Static members** (methods and variables) belong to the class rather than any object of the class. They can be accessed directly using the class name.

### 7. What is the use of `super` and `this` keywords?

- **`this`**: Refers to the current object instance.
- **`super`**: Refers to the superclass object.

### 8. What are access modifiers in Java?

Java has four access modifiers:

- **public**: Accessible from anywhere.
- **protected**: Accessible within the package and subclasses.
- **default**: Accessible only within the package.
- **private**: Accessible only within the class.

### 9. What is the difference between a constructor and a method?

- **Constructor**: Initializes an object when it is created.
- **Method**: A block of code that performs a specific task when called.

---

## Conclusion

This `README` covers the essential Java concepts and the most common interview questions with their answers. Understanding these topics thoroughly will help you in your upcoming placement drives.
