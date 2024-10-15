# Object-Oriented Programming (OOP) Concepts in Java

This README is a comprehensive guide to Object-Oriented Programming (OOP) concepts in Java. It covers all essential topics, providing examples, explanations, and important interview questions to prepare you for placement drives.

## Table of Contents

1. [What is OOP?](#what-is-oop)
2. [Core OOP Concepts](#core-oop-concepts)
   - [Class and Object](#class-and-object)
   - [Abstraction](#abstraction)
   - [Encapsulation](#encapsulation)
   - [Inheritance](#inheritance)
   - [Polymorphism](#polymorphism)
3. [Other Important Concepts](#other-important-concepts)
   - [Association](#association)
   - [Aggregation](#aggregation)
   - [Composition](#composition)
   - [Static Members](#static-members)
4. [Sample Code](#sample-code)
5. [Common Interview Questions](#common-interview-questions)

---

## What is OOP?

**Object-Oriented Programming (OOP)** is a programming paradigm based on the concept of "objects," which contain data and methods. OOP promotes code reusability, scalability, and efficiency.

### Why use OOP?

- **Modularity**: Break down large programs into smaller, manageable objects.
- **Reusability**: Reuse objects across different programs or parts of the same program.
- **Data Security**: Encapsulation keeps the data safe and secure from outside access.

---

## Core OOP Concepts

### 1. Class and Object

- A **class** is a blueprint or template that defines objects.
- An **object** is an instance of a class.

```java
class Car {
    String color;
    String model;

    void drive() {
        System.out.println("The " + color + " " + model + " is driving");
    }
}

public class Main {
    public static void main(String[] args) {
        Car myCar = new Car(); // Creating an object
        myCar.color = "Red";
        myCar.model = "Tesla";
        myCar.drive(); // Output: The Red Tesla is driving
    }
}
```

### 2. Abstraction

- **Abstraction** is hiding the implementation details and showing only the necessary parts of an object.

```java
abstract class Animal {
    abstract void sound();
}

class Dog extends Animal {
    void sound() {
        System.out.println("Dog barks");
    }
}
```

### 3. Encapsulation

- **Encapsulation** is bundling the data (variables) and methods (functions) into a single unit (class) and restricting outside access using access modifiers (`private`, `public`).

```java
class Person {
    private String name; // Private variable

    public void setName(String name) { // Setter method
        this.name = name;
    }

    public String getName() { // Getter method
        return this.name;
    }
}
```

### 4. Inheritance

- **Inheritance** allows a new class to inherit properties and behavior (methods) from an existing class.

```java
class Vehicle {
    void start() {
        System.out.println("Vehicle started");
    }
}

class Car extends Vehicle {
    void honk() {
        System.out.println("Car honks");
    }
}
```

### 5. Polymorphism

- **Polymorphism** allows methods to have the same name but behave differently based on the object.

#### Method Overloading (Compile-time Polymorphism)

```java
class MathOperations {
    int add(int a, int b) {
        return a + b;
    }

    double add(double a, double b) {
        return a + b;
    }
}
```

#### Method Overriding (Runtime Polymorphism)

```java
class Cat extends Animal {
    void sound() {
        System.out.println("Cat meows");
    }
}
```

---

## Other Important Concepts

### 1. Association

- **Association** defines a relationship between two separate classes that work together.

### 2. Aggregation

- **Aggregation** is a type of association where one class owns another class but both can exist independently.

```java
class Department {
    String deptName;
    Department(String deptName) {
        this.deptName = deptName;
    }
}
class University {
    String universityName;
    List<Department> departments; // Aggregation

    University(String name) {
        this.universityName = name;
    }
}
```

### 3. Composition

- **Composition** is a type of association where one class cannot exist without the other.

```java
class Engine {
    Engine() {
        System.out.println("Engine started");
    }
}
class Car {
    Engine engine; // Composition

    Car() {
        engine = new Engine();
    }
}
```

### 4. Static Members

- **Static members** belong to the class rather than an instance of the class. They can be accessed without creating an object.

```java
class Calculator {
    static int add(int a, int b) {
        return a + b;
    }
}

public class Main {
    public static void main(String[] args) {
        System.out.println("Sum: " + Calculator.add(10, 15)); // Output: 25
    }
}
```

---

## Sample Code

Here’s a sample Java code that demonstrates all the above OOP concepts.

```java
// OOP Concepts in Java

// 1. Class and Object Example
class Car {
    String color;
    String model;

    void drive() {
        System.out.println("The " + color + " " + model + " is driving");
    }
}

public class MainOOP {
    public static void main(String[] args) {
        // Class and Object Example
        Car myCar = new Car(); // Creating an object
        myCar.color = "Red";
        myCar.model = "Tesla";
        myCar.drive(); // Output: The Red Tesla is driving

        // Abstraction and Inheritance Example
        Dog dog = new Dog();
        dog.sound(); // Output: Dog barks

        // Encapsulation Example
        Person person = new Person();
        person.setName("John");
        System.out.println(person.getName()); // Output: John

        // Polymorphism Example (Method Overloading)
        MathOperations math = new MathOperations();
        System.out.println("Sum of integers: " + math.add(10, 20)); // Output: 30
        System.out.println("Sum of doubles: " + math.add(10.5, 20.5)); // Output: 31.0

        // Polymorphism Example (Method Overriding)
        Animal myAnimal = new Dog();
        myAnimal.sound(); // Output: Dog barks

        // Static Members Example
        System.out.println("Sum using static method: " + Calculator.add(10, 15)); // Output: 25
    }
}

// 2. Abstraction Example
abstract class Animal {
    abstract void sound();
}

class Dog extends Animal {
    void sound() {
        System.out.println("Dog barks");
    }
}

// 3. Encapsulation Example
class Person {
    private String name; // Private variable

    public void setName(String name) { // Setter method
        this.name = name;
    }

    public String getName() { // Getter method
        return this.name;
    }
}

// 4. Inheritance Example
class Vehicle {
    void start() {
        System.out.println("Vehicle started");
    }
}

class Car2 extends Vehicle {
    void honk() {
        System.out.println("Car honks");
    }
}

// 5. Polymorphism Example
// Compile-time Polymorphism (Method Overloading)
class MathOperations {
    int add(int a, int b) {
        return a + b;
    }

    double add(double a, double b) {
        return a + b;
    }
}

// Runtime Polymorphism (Method Overriding)
class Cat extends Animal {
    void sound() {
        System.out.println("Cat meows");
    }
}

// 6. Association, Aggregation, and Composition
class University {
    String universityName;

    University(String name) {
        this.universityName = name;
    }
}
```

---

## Common Interview Questions

Here are some important OOP-related interview questions you should prepare for:

# OOPs Concepts: Interview Questions and Answers

1. **What is the difference between abstraction and encapsulation?**

   - **Abstraction**: Hides implementation details and shows only functionality. It is implemented using abstract classes or interfaces.
   - **Encapsulation**: Encloses the data (variables) and methods in a single unit, typically a class, and restricts access using access modifiers.

2. **Explain inheritance and its types.**

   - **Inheritance**: A mechanism where one class acquires properties (fields) and behaviors (methods) of another class.
     - **Single Inheritance**: A subclass inherits from one superclass.
     - **Multiple Inheritance (Java doesn’t support)**: A class inherits from more than one class.
     - **Multilevel Inheritance**: A class inherits from a class, which in turn inherits from another class.
     - **Hierarchical Inheritance**: Multiple subclasses inherit from a single class.
     - **Hybrid Inheritance**: Combination of two or more types of inheritance.

3. **What is method overloading and method overriding?**

   - **Method Overloading**: Multiple methods with the same name but different parameter lists (either in type, number, or order) in the same class.
   - **Method Overriding**: Redefining a method in the subclass that already exists in the superclass with the same signature (name and parameters).

4. **What is the difference between association, aggregation, and composition?**

   - **Association**: A general relationship between two classes where one uses the other.
   - **Aggregation**: A weak association where one class owns another but can exist independently.
   - **Composition**: A strong association where one class cannot exist without the other (e.g., a house cannot exist without rooms).

5. **How is polymorphism achieved in Java?**

   - **Polymorphism**: The ability to perform a single action in different ways.
     - **Compile-time polymorphism**: Achieved through method overloading.
     - **Run-time polymorphism**: Achieved through method overriding.

6. **What are static members in Java?**

   - **Static members** are class-level members (variables or methods) that belong to the class rather than instances of the class. They can be accessed without creating an object.

7. **Explain the use of `super` and `this` keywords in Java.**

   - **'this' keyword**: Refers to the current instance of the class. Used to differentiate between class variables and parameters.
   - **'super' keyword**: Refers to the parent class and is used to call parent class methods or constructors.

8. **What is an abstract class and how is it different from an interface?**

   - **Abstract class**: A class that cannot be instantiated on its own and may contain abstract and non-abstract methods. It is used to share common functionality.
   - **Interface**: A contract where classes must implement abstract methods defined in it. Before Java 8, interfaces couldn't have any concrete methods.

9. **What are access modifiers in Java?**

   - **Access Modifiers** control the visibility of class members. Java has four:
     - **Private**: Visible only within the same class.
     - **Default**: Visible within the same package.
     - **Protected**: Visible within the same package and subclasses.
     - **Public**: Visible from any class.

10. **What is the difference between a constructor and a method?**

- **Constructor**: A special method invoked when an object is created. It doesn't have a return type and is used to initialize objects.
- **Method**: A regular function defined in a class, used to perform actions, and may or may not return a value.

---

### **Good Luck!**

This file covers the fundamentals of OOP concepts and important interview questions. It should help you strengthen your understanding of OOP in Java!
