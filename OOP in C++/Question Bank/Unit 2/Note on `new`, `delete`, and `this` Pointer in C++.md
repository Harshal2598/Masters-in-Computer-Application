# Note on `new`, `delete`, and `this` Pointer in C++

Dynamic memory allocation in C++ is achieved using the **new**, **delete**, and sometimes the **this** pointer.  
These allow a program to allocate memory at runtime and manage objects efficiently.

---

# 1️⃣ `new` Operator

`new` is used to **allocate memory dynamically** during program execution.

### ✔ Features
- Allocates memory from the **heap**
- Returns a **pointer** to the allocated memory
- Can allocate memory for:
  - A single variable
  - An array
  - Objects

### ✔ Example
```cpp
int *p = new int;   // allocate memory for 1 integer
*p = 10;
```

### ✔ Example: Dynamic Array
```cpp
int *arr = new int[5];   // array of size 5
```

---

# 2️⃣ `delete` Operator

`delete` is used to **free** dynamically allocated memory.  
It prevents **memory leaks**.

### ✔ Features
- Frees memory allocated by `new`
- `delete` → for single variable
- `delete[]` → for arrays

### ✔ Example
```cpp
delete p;       // free single variable
delete[] arr;   // free array
```

---

# 3️⃣ `this` Pointer

`this` is an **implicit pointer** available inside every non-static member function.  
It stores the **address of the current calling object**.

### ✔ Uses of `this` Pointer
- To access current object’s data members  
- To distinguish between **local** and **instance** variables  
- Useful in dynamic memory allocation when objects are created using `new`  
- Used for returning the current object (method chaining)

### ✔ Example
```cpp
class Demo {
    int x;

public:
    Demo(int x) {
        this->x = x;     // 'this' refers to the current object
    }

    void show() {
        cout << "Value = " << this->x;
    }
};
```

---

# ⭐ Example Program Using `new`, `delete`, and `this`

```cpp
#include <iostream>
using namespace std;

class Student {
    int marks;

public:
    Student(int marks) {
        this->marks = marks;      // using this pointer
    }

    void display() {
        cout << "Marks = " << this->marks << endl;
    }
};

int main() {
    Student *s = new Student(90);   // dynamic object creation

    s->display();

    delete s;   // free memory
    return 0;
}
```

---

# ⭐ Summary Table

| Feature | Description |
|---------|-------------|
| `new` | Allocates memory dynamically and returns pointer |
| `delete` | Frees memory allocated by new |
| `this` pointer | Points to the current object and used to access members |

---

# 🎯 Conclusion

- **new** and **delete** provide flexible memory management at runtime.  
- **this** pointer helps refer to the current object, especially in constructors and dynamic objects.  
- Together, they form an essential part of **dynamic memory allocation** and **OOP programming** in C++.

