# Operators in C++

Operators in C++ are symbols used to perform operations on variables and values.  
They help in calculations, comparisons, logical operations, and memory handling.

C++ provides the following categories of operators:

---

# 1️⃣ Arithmetic Operators

Used to perform mathematical operations.

| Operator | Meaning | Example |
|---------|----------|---------|
| `+` | Addition | `a + b` |
| `-` | Subtraction | `a - b` |
| `*` | Multiplication | `a * b` |
| `/` | Division | `a / b` |
| `%` | Modulus | `a % b` |

### Example:
```cpp
int a = 10, b = 3;
cout << a % b;  // Output: 1
```

---

# 2️⃣ Relational Operators

Used to compare two values.  
Result: **true (1)** or **false (0)**.

| Operator | Meaning | Example |
|----------|---------|---------|
| `==` | Equal to | `a == b` |
| `!=` | Not equal | `a != b` |
| `>` | Greater than | `a > b` |
| `<` | Less than | `a < b` |
| `>=` | Greater or equal | `a >= b` |
| `<=` | Less or equal | `a <= b` |

### Example:
```cpp
cout << (5 > 3);  // Output: 1
```

---

# 3️⃣ Logical Operators

Used for logical (Boolean) operations.

| Operator | Meaning | Example |
|----------|---------|---------|
| `&&` | Logical AND | `(a > 0 && b > 0)` |
| `||` | Logical OR | `(a > 0 || b > 0)` |
| `!` | Logical NOT | `!a` |

### Example:
```cpp
cout << (5 > 3 && 3 > 2);  // Output: 1
```

---

# 4️⃣ Assignment Operators

Used to assign values.

| Operator | Meaning | Example |
|----------|---------|---------|
| `=` | Assign | `a = 10` |
| `+=` | Add & assign | `a += 5` |
| `-=` | Subtract & assign | `a -= 3` |
| `*=` | Multiply & assign | `a *= 2` |
| `/=` | Divide & assign | `a /= 2` |
| `%=` | Modulus & assign | `a %= 2` |

### Example:
```cpp
int a = 10;
a += 5;  // a = 15
```

---

# 5️⃣ Increment & Decrement Operators

Used to increase or decrease value by 1.

| Operator | Meaning |
|----------|----------|
| `++` | Increment |
| `--` | Decrement |

### Example:
```cpp
int x = 5;
cout << ++x;  // Output: 6
```

---

# 6️⃣ Bitwise Operators

Used for operations on bits (0s and 1s).

| Operator | Meaning |
|----------|---------|
| `&` | Bitwise AND |
| `|` | Bitwise OR |
| `^` | XOR |
| `~` | Bitwise NOT |
| `<<` | Left shift |
| `>>` | Right shift |

### Example:
```cpp
cout << (5 & 3);  // Output: 1
```

---

# 7️⃣ Conditional (Ternary) Operator

Short form of if-else.

### Syntax:
```cpp
condition ? value_if_true : value_if_false
```

### Example:
```cpp
int a = 10, b = 20;
int max = (a > b) ? a : b;
```

---

# 8️⃣ Sizeof Operator

Used to find the size of a data type or variable.

### Example:
```cpp
cout << sizeof(int);  // Output: 4
```

---

# 9️⃣ Scope Resolution Operator `::`

Used to access global variables or class members.

### Example:
```cpp
int x = 10;
::x;  // accesses global x
```

---

# 🔟 Member Access Operators

Used inside classes and objects.

| Operator | Meaning |
|----------|---------|
| `.` | Access object members |
| `->` | Access pointer object members |

### Example:
```cpp
obj.show();
ptr->display();
```

---

# ⭐ Summary

C++ supports various operators that help perform arithmetic, logical, comparison, assignment, bit-level, and object-oriented operations.  
They make programs efficient and expressive.

