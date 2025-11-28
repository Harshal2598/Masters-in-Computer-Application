# Dynamic Memory Allocation in C++

Dynamic Memory Allocation in C++ means **allocating memory at runtime (during program execution)** instead of compile time.  
This allows programs to use exactly the amount of memory needed, making memory usage flexible and efficient.

C++ uses two operators for dynamic memory:

- `new` → allocates memory  
- `delete` → frees memory  

---

# ⭐ Why Dynamic Memory Allocation?

- Exact memory requirement is **unknown** until runtime  
- Efficient use of memory  
- Useful in:
  - Arrays with variable size  
  - Linked lists, trees, graphs  
  - Large data structures  

---

# 1️⃣ `new` Operator

Used to **dynamically allocate memory** for variables and arrays.

### ✔ Syntax
```cpp
pointer = new dataType;
```

### ✔ Example: Allocating an Integer
```cpp
int *p = new int;  // memory allocated for 1 integer
*p = 10;
cout << *p;
```

---

# 2️⃣ `delete` Operator

Used to **free (deallocate) memory** allocated using `new`.

### ✔ Syntax
```cpp
delete pointer;
```

### ✔ Example
```cpp
delete p;   // frees memory
```

---

# ✔ Complete Example: Single Variable Allocation
```cpp
#include <iostream>
using namespace std;

int main() {
    int *ptr = new int;   // dynamic allocation
    *ptr = 25;

    cout << "Value = " << *ptr << endl;

    delete ptr;           // free memory
    return 0;
}
```

---

# 3️⃣ Dynamic Allocation of Arrays

### ✔ Syntax
```cpp
pointer = new dataType[size];
```

### ✔ Example: Dynamic Array
```cpp
int n;
cout << "Enter size: ";
cin >> n;

int *arr = new int[n];   // dynamic array

for (int i = 0; i < n; i++) {
    arr[i] = i + 1;
}

for (int i = 0; i < n; i++) {
    cout << arr[i] << " ";
}

delete[] arr;            // delete dynamic array
```

---

# 4️⃣ Important Notes

- Always use `delete` or `delete[]` to avoid **memory leaks**  
- `new` returns a pointer  
- `delete[]` is used **only for arrays created using new[]**

---

# ⭐ Summary

| Feature | `new` | `delete` |
|--------|--------|-----------|
| Purpose | Allocate memory | Free memory |
| Returns | Pointer | Nothing |
| Used For | Variables & arrays | Variables & arrays |
| Syntax | `ptr = new int;` | `delete ptr;` |

---

# 🎯 Conclusion

Dynamic memory allocation in C++ provides flexibility to allocate memory at runtime using `new` and free it using `delete`.  
It is essential for creating efficient programs, especially when working with data structures like linked lists, trees, and graphs.

