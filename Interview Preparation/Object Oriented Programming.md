
---

### **1) What is OOPS?**

**OOPS (Object-Oriented Programming System)** is a programming approach where software is designed using objects. Each object is an instance of a class and contains data (attributes) and behavior (methods).

---

### **2) What are the basic concepts of OOPS?**

The four main concepts of OOPS are:

1. **Abstraction** – Hiding unnecessary details and showing only the essential parts.
2. **Encapsulation** – Wrapping data and code together to protect it from direct access.
3. **Inheritance** – Allowing one class to use the properties and methods of another class.
4. **Polymorphism** – Ability to take multiple forms, allowing methods to perform different tasks based on input.

---

### **3) What is a class?**

A **class** is a blueprint for creating objects. It defines attributes (variables) and behaviors (methods) that the objects will have.  
Example:

```java
class Car {
    String color;
    void drive() {
        System.out.println("Car is moving");
    }
}
```

---

### **4) What is an Object?**

An **object** is an instance of a class. It has its own values for the attributes and can perform actions (methods).  
Example:

```java
Car myCar = new Car();  // Creating an object of the Car class
myCar.color = "Red";  // Assigning value to an object
```

---

### **5) What is Encapsulation?**

Encapsulation means **hiding data** from direct access and only allowing it through methods. It ensures security and prevents unauthorized modification.  
Example:

```java
class BankAccount {
    private double balance;  // Private variable (hidden)

    public void deposit(double amount) {  // Public method to access private data
        balance += amount;
    }
}
```

---

### **6) What is Polymorphism?**

Polymorphism allows methods to have different behaviors based on input. It is of two types:

- **Method Overloading** – Multiple methods with the same name but different parameters.
- **Method Overriding** – A subclass provides a specific implementation of a method from its parent class.

Example:

```java
// Method Overloading
class MathOperations {
    int add(int a, int b) { return a + b; }
    double add(double a, double b) { return a + b; }
}
```

---

### **7) What is Inheritance?**

Inheritance allows a class (child) to inherit properties and methods from another class (parent).  
Types of Inheritance:

- **Single Inheritance** – One class inherits from another.
- **Multiple Inheritance (not in Java)** – A class inherits from multiple classes.
- **Multilevel Inheritance** – A class inherits from another class, which in turn inherits from another.
- **Hierarchical Inheritance** – Multiple child classes inherit from a single parent class.

Example:

```java
class Animal {
    void sound() { System.out.println("Animal makes a sound"); }
}

class Dog extends Animal {
    void sound() { System.out.println("Dog barks"); }
}
```

---

### **8) What are manipulators?**

Manipulators are functions used with **input (>>) and output (<<) operators** to format data in C++.  
Example: `endl` (new line) and `setw` (set width).

---

### **9) What is a Constructor?**

A **constructor** is a special method that initializes an object when it is created. It has the same name as the class and has no return type.  
Example:

```java
class Person {
    String name;
    Person() {  // Constructor
        name = "Default Name";
    }
}
```

---

### **10) What is a Destructor?**

A **destructor** is a method that is automatically called when an object is destroyed. In Java, this is handled by the **Garbage Collector** using the `finalize()` method.  
Example:

```java
class Test {
    protected void finalize() { System.out.println("Object destroyed"); }
}
```

---

### **11) What is an Inline Function?**

An **inline function** tells the compiler to replace the function call with the function code itself, reducing function call overhead. Used in C++, not in Java.

---

### **12) What is a Virtual Function?**

A **virtual function** is a method that can be overridden in a subclass and supports runtime polymorphism. It is used in C++ with the `virtual` keyword.

---

### **13) What is a Friend Function?**

A **friend function** is a function that is not part of a class but can access its private and protected members. This is mainly in C++.

---

### **14) What is Function Overloading?**

Function overloading allows multiple methods with the **same name but different parameters** in the same class.  
Example:

```java
class Math {
    void add(int a, int b) { System.out.println(a + b); }
    void add(double a, double b) { System.out.println(a + b); }
}
```

---

### **15) What is Operator Overloading?**

**Operator overloading** allows custom behavior for operators like `+`, `-`, etc., but **Java does not support this feature** (only C++ does).

---

### **16) What is an Abstract Class?**

An **abstract class** cannot be instantiated and is used as a base for other classes. It can contain **abstract methods** (methods without a body).  
Example:

```java
abstract class Vehicle {
    abstract void start();  // Abstract method (no body)
}

class Car extends Vehicle {
    void start() { System.out.println("Car starts with key"); }
}
```

---

### **17) What is a Ternary Operator?**

A **ternary operator** is a shorthand for `if-else`.  
Syntax:

```java
int result = (a > b) ? a : b;  // If a > b, result = a; else result = b
```

---

### **18) What is the use of the Finalize Method?**

The `finalize()` method is called before an object is **garbage collected**. It is used to **clean up resources** like file handles or database connections.  
Example:

```java
protected void finalize() { System.out.println("Object is being destroyed"); }
```

---

### **19) What are the different types of Arguments?**

1. **Call by Value** – A copy of the argument is passed, and changes do not affect the original value.
2. **Call by Reference** – The actual argument is passed, and changes affect the original value.

Example:

```java
void callByValue(int x) { x = 10; }  // Original x remains unchanged
void callByReference(int[] arr) { arr[0] = 10; }  // Changes original array
```

---

### **20) What is the Super Keyword?**

The `super` keyword refers to the **parent class** and is used to access its methods or constructor.  
Example:

```java
class Parent {
    void display() { System.out.println("Parent method"); }
}

class Child extends Parent {
    void display() {
        super.display();  // Calls parent class method
        System.out.println("Child method");
    }
}
```

---

Here's the cleaned-up version of your content with proper spacing and formatting for easier readability:

---

**21) What is method overriding?**  
Method overriding is a feature that allows a subclass to provide the implementation of a method that is already defined in the superclass. It will override the implementation in the superclass by providing the same method name, same parameters, and the same return type.

**22) What is an interface?**  
An interface is a collection of abstract methods. If a class implements an interface, it inherits all the abstract methods of that interface. Java uses interfaces to implement multiple inheritance.

**23) What is exception handling?**  
An exception is an event that occurs during the execution of a program. Exceptions can be of any type, such as RuntimeException or Error exceptions. These exceptions are adequately handled through exception handling mechanisms like try, catch, and throw keywords.

**24) What are tokens?**  
A compiler recognizes a token, which cannot be broken down into component elements. Keywords, identifiers, constants, string literals, and operators are examples of tokens. Even punctuation characters like brackets, commas, braces, and parentheses are considered tokens.

**25) What is the main difference between overloading and overriding?**  
Overloading is static binding, while overriding is dynamic binding.

- Overloading refers to having the same method name with different arguments in the same class. It may or may not return the same value.
- Overriding refers to having the same method name, same arguments, and same return type in the parent class and its child class.

**26) What is the main difference between a class and an object?**  
An object is an instance of a class. Objects hold multiple pieces of information, while classes do not have any data. Definitions of properties and functions are done in classes, which can be used by objects.  
A class can have subclasses, but an object does not have sub-objects.

**27) What is abstraction?**  
Abstraction is an OOP feature that shows only the necessary details to the client of an object. It hides the inner workings or implementation.  
Example: When you switch on a television, you don’t need to know the inner circuitry, just how to turn it on.

**28) What are access modifiers?**  
Access modifiers determine the scope of methods or variables that can be accessed from other classes or objects. There are five types of access modifiers:

- Private
- Protected
- Public
- Friend
- Protected Friend

**29) What are sealed modifiers?**  
Sealed modifiers are access modifiers where methods cannot be inherited. Sealed modifiers can be applied to properties, events, and methods. This modifier cannot be used for static members.

**30) How can we call the base method without creating an instance?**  
Yes, it is possible to call the base method without creating an instance, if the method is static. Use the `Base` keyword from a derived class when doing inheritance.

**31) What is the difference between `new` and `override`?**  
The `new` modifier instructs the compiler to use the new implementation instead of the base class function. The `override` modifier is used to override the base class function.

**32) What are the various types of constructors?**  
There are three types of constructors:

- Default Constructor: No parameters.
- Parametric Constructor: With parameters, creates a new instance while passing arguments.
- Copy Constructor: Creates a new object as a copy of an existing object.

**33) What is early and late binding?**  
Early binding refers to the assignment of values to variables during design time, whereas late binding occurs during runtime.

**34) What is the `this` pointer?**  
The `this` pointer refers to the current object of a class. It differentiates between the current object and the global object.

**35) What is the difference between structure and class?**  
The default access type of a structure is public, while the default access type of a class is private.  
A structure is used for grouping data, while a class is used for grouping data and methods. Structures are exclusively used for data and don't require strict validation, while classes encapsulate data and require strict validation.

**36) What is the default access modifier in a class?**  
The default access modifier for a class is `internal`, and the default access modifier for a class member is `private`.

**37) What is a pure virtual function?**  
A pure virtual function is a function that can be overridden in a derived class but cannot be defined in the base class. It is declared using `= 0`.  
Example:  
`Virtual void function1()` // Virtual, Not pure  
`Virtual void function2() = 0` // Pure virtual

**38) What are all the operators that cannot be overloaded?**  
The following operators cannot be overloaded:

1. Scope Resolution (`::`)
2. Member Selection (`.`)
3. Member Selection through a pointer to a function (`.*`)

**39) What is dynamic or runtime polymorphism?**  
Dynamic or runtime polymorphism is also known as method overriding. It resolves calls to an overridden function during runtime, not compile-time. This allows having methods with the same name and signature but different implementations.

**40) Do we require a parameter for constructors?**  
No, parameters are not required for constructors. Constructors can be defined with or without parameters.

**41) What is a copy constructor?**  
A copy constructor is a special constructor used to create a new object as a copy of an existing object. There can be only one copy constructor, which can be either defined by the user or the system.

**42) What does the keyword `virtual` represent in a method definition?**  
The `virtual` keyword means that the method can be overridden in derived classes.

**43) Can a static method use non-static members?**  
No, a static method cannot use non-static members.

**44) What are base class, subclass, and superclass?**

- A base class is the most generalized class, also called a root class.
- A subclass is a class that inherits from one or more base classes.
- A superclass is the parent class from which another class inherits.

**45) What is static and dynamic binding?**  
Binding refers to associating a name with a class.

- Static binding (or early binding) happens at compile-time.
- Dynamic binding (or late binding) happens at runtime.

**46) How many instances can be created for an abstract class?**  
No instances can be created for an abstract class. You cannot create an instance of an abstract class.

**47) Which keyword can be used for overloading?**  
The `operator` keyword can be used for overloading operators.

**48) What is the default access specifier in a class definition?**  
The default access specifier in a class definition is `private`.

**49) Which OOPS concept is used as a reuse mechanism?**  
Inheritance is the OOPS concept used as a reuse mechanism.

**50) Which OOPS concept exposes only the necessary information to the calling functions?**  
Encapsulation exposes only the necessary information to the calling functions.

---
Here are the questions from sequence 51:

**Q 51. What is a Virtual Function?**

A **virtual function** is a function in the base class that can be overridden by a derived class. When a function is declared as virtual, it tells the compiler to look at the object's actual type (not the type of the pointer or reference) to determine which function to call. This supports **runtime polymorphism**, allowing the program to decide which function to invoke at runtime.

In C++:

```cpp
#include <iostream>
using namespace std;

class Animal {
public:
    virtual void sound() {
        cout << "Animal makes a sound" << endl;
    }
};

class Dog : public Animal {
public:
    void sound() override {
        cout << "Dog barks" << endl;
    }
};

int main() {
    Animal* animal = new Dog();
    animal->sound();  // Output: Dog barks
    delete animal;
    return 0;
}
```

**Q 52. What is the difference between a static and dynamic function call?**

- **Static function call**: The function call is resolved at compile time. The function call is linked to the method in the code when the program is compiled.
    
- **Dynamic function call**: The function call is resolved at runtime. It happens when the type of the object is determined at runtime and the appropriate method is invoked.
    

**Q 53. What is a friend function?**

A **friend function** is a function that is not a member of a class but has access to its private and protected members. It can access all the data members and methods of the class it is a friend of.

Example in C++:

```cpp
class Box {
private:
    int width;
public:
    Box() { width = 10; }
    friend void printWidth(Box);  // Friend function declaration
};

void printWidth(Box b) {
    cout << "Width: " << b.width << endl;  // Can access private member
}

int main() {
    Box box;
    printWidth(box);  // Output: Width: 10
    return 0;
}
```

**Q 54. What is the purpose of the `this` pointer in C++?**

The **`this` pointer** is a special pointer available to non-static member functions of a class. It points to the current object of the class. It allows a function to refer to the object that called it, which can be useful when differentiating between member variables and parameters.

Example:

```cpp
class Test {
private:
    int value;
public:
    Test(int value) {
        this->value = value;  // The `this` pointer is used to refer to the member variable
    }
};
```

**Q 55. What are Lambda expressions in C++?**

A **Lambda expression** is an anonymous function that can be defined at the point where it is used. Lambda expressions allow defining functions inline and are useful for short functions that are used only once.

Syntax:

```cpp
[ capture_clause ] ( parameter_list ) -> return_type { body }
```

Example:

```cpp
#include <iostream>
using namespace std;

int main() {
    auto sum = [](int a, int b) -> int {
        return a + b;
    };
    
    cout << sum(3, 4);  // Output: 7
    return 0;
}
```

**Q 56. What is the difference between `new` and `malloc`?**

- **`new`**: Allocates memory for a single object or array of objects. It calls the constructor of the class to initialize the object(s).
- **`malloc`**: Allocates a block of memory for the specified number of bytes but does not initialize the memory. It returns a pointer to the allocated memory.

Example:

```cpp
int* arr1 = new int[10];   // Allocates memory for 10 integers
int* arr2 = (int*)malloc(10 * sizeof(int));  // Allocates memory for 10 integers, but does not initialize
```

**Q 57. What is a Smart Pointer in C++?**

A **smart pointer** is an object that behaves like a pointer but automatically manages the memory it points to. When the smart pointer goes out of scope, it automatically frees the memory, preventing memory leaks.

Types of smart pointers:

- **`std::unique_ptr`**: A smart pointer that owns a dynamically allocated object and ensures it is deleted when no longer needed.
- **`std::shared_ptr`**: A smart pointer that allows multiple pointers to share ownership of the same object.
- **`std::weak_ptr`**: A smart pointer that doesn’t affect the reference count of an object managed by `shared_ptr`.

Example using `std::unique_ptr`:

```cpp
#include <iostream>
#include <memory>
using namespace std;

int main() {
    unique_ptr<int> ptr = make_unique<int>(10);
    cout << *ptr << endl;  // Output: 10
    return 0;
}
```

**Q 58. What is a reference in C++?**

A **reference** is an alias for another variable. It allows you to access the value of a variable without creating a copy. It must be initialized when declared and cannot be made to refer to another variable after that.

Example:

```cpp
int a = 10;
int& ref = a;  // 'ref' is now a reference to 'a'

ref = 20;  // Changes the value of 'a' to 20
cout << a;  // Output: 20
```

**Q 59. What is an exception in C++?**

An **exception** is a runtime error that occurs during program execution. C++ provides a mechanism for handling exceptions using `try`, `throw`, and `catch` blocks.

Example:

```cpp
#include <iostream>
using namespace std;

int main() {
    try {
        int num = 0;
        if (num == 0) {
            throw "Division by zero error!";
        }
    }
    catch (const char* msg) {
        cout << msg << endl;  // Output: Division by zero error!
    }
    return 0;
}
```

**Q 60. What is a namespace in C++?**

A **namespace** is a feature that allows grouping identifiers (such as variables, functions, classes) to avoid name conflicts, especially in large programs or when combining code from different libraries.

Example:

```cpp
namespace Math {
    int add(int a, int b) {
        return a + b;
    }
}

int main() {
    cout << Math::add(2, 3);  // Output: 5
    return 0;
}
```


#### 61. **What is Composition?**

Composition is a specialized form of aggregation where the part cannot exist without the whole. It implies a strong relationship, and if the whole object is destroyed, its parts are also destroyed.

#### 62. **What is Aggregation?**

Aggregation is a "HAS-A" relationship. It’s a weak relationship where one object (the whole) contains references to other objects (the parts), but the parts can exist independently of the whole.

#### 63. **What is Dependency?**

Dependency occurs when one class relies on another to perform certain tasks. This is represented by one class having a reference or dependency on another class.

#### 64. **What is the difference between Association and Dependency?**

- **Association** is a broad term where one class contains a reference to another.
- **Dependency** is a more specific term, referring to a situation where one class's method depends on another class for its functionality.

