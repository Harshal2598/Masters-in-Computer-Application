# Pillars of Object-Oriented Programming (OOP)

Object-Oriented Programming is built on **four main pillars** that define how objects and classes interact.  
These pillars make software **modular, reusable, secure, and easy to maintain**.

---

# 1️⃣ **Encapsulation**

Encapsulation means **wrapping data and methods into a single unit** (class) and **protecting** the data from outside interference.

### ✔ Key Points
- Hides internal details using `private` access
- Exposes controlled access using getters and setters
- Prevents accidental data modification
- Improves security

### ✔ Example
```java
class Student {
    private int marks;  // hidden data

    public void setMarks(int m) {  
        marks = m;  // controlled access
    }

    public int getMarks() {
        return marks;
    }
}
```

### ✔ In simple words:
> Encapsulation = Data hiding + controlled access.

---

# 2️⃣ **Inheritance**

Inheritance allows a class to **acquire properties and methods of another class**.  
It supports code **reusability** and helps create hierarchical relationships.

### ✔ Key Points
- Reduces code duplication  
- Parent class (superclass) → Child class (subclass)  
- Child can use and extend parent's features

### ✔ Example
```java
class Animal {
    void eat() { System.out.println("Eating"); }
}

class Dog extends Animal {
    void bark() { System.out.println("Barking"); }
}
```

### ✔ In simple words:
> Inheritance = Reusing existing code.

---

# 3️⃣ **Polymorphism**

Polymorphism means **one name, many forms**.  
It allows the same function or method to work in **different ways**.

There are two types:

### ✔ (A) Compile-Time Polymorphism (Method Overloading)
```java
void show(int a) {}
void show(String b) {}
```

### ✔ (B) Run-Time Polymorphism (Method Overriding)
```java
class Animal { void sound(){ System.out.println("Sound"); } }
class Dog extends Animal { void sound(){ System.out.println("Bark"); } }
```

### ✔ In simple words:
> Polymorphism = Same action, different behavior.

---

# 4️⃣ **Abstraction**

Abstraction means **showing only essential details** and **hiding complex implementation**.

### ✔ Key Points
- Achieved using **abstract classes** and **interfaces**
- Reduces complexity
- Helps focus on behavior, not details

### ✔ Example
```java
abstract class Car {
    abstract void drive();  // important action only
}

class Tesla extends Car {
    void drive() { System.out.println("Self-driving mode"); }
}
```

### ✔ In simple words:
> Abstraction = Hide complexity, show functionality.

---

# ⭐ Summary Table

| Pillar | Meaning | Benefit |
|--------|---------|----------|
| Encapsulation | Hide data using classes | Security |
| Inheritance | Reuse parent class features | Code reusability |
| Polymorphism | Same name, different behavior | Flexibility |
| Abstraction | Show essential features only | Reduced complexity |

---

# 🎯 Conclusion
The 4 pillars of OOP make programming more organized, secure, reusable, and easier to maintain.  
Any object-oriented language (Java, C++, Python, C#) is built on these fundamental principles.

