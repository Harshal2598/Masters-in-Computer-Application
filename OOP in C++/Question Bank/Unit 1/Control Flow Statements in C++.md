# Control Flow Statements in C++

Control flow statements determine **the order in which statements are executed** in a program.  
They allow a program to **make decisions**, **repeat tasks**, and **control execution flow** based on conditions.

C++ provides three major categories of control flow statements:

1. **Selection (Decision) Statements**  
2. **Iteration (Looping) Statements**  
3. **Jump Statements**

---

# 1️⃣ Selection (Decision) Statements

These statements allow the program to **choose a path** based on conditions.

---

## ✔ `if` Statement
Executes a block only if the condition is true.

### Example:
```cpp
int age = 20;
if (age >= 18) {
    cout << "Eligible to vote";
}
```

---

## ✔ `if-else` Statement
Chooses between two blocks based on a condition.

### Example:
```cpp
int marks = 40;
if (marks >= 35)
    cout << "Pass";
else
    cout << "Fail";
```

---

## ✔ `else-if` Ladder
Used to check multiple conditions.

### Example:
```cpp
int marks = 85;

if (marks >= 90)
    cout << "Grade A";
else if (marks >= 75)
    cout << "Grade B";
else
    cout << "Grade C";
```

---

## ✔ `switch` Statement
Used when multiple conditions depend on the **same variable**.

### Example:
```cpp
int choice = 2;

switch (choice) {
    case 1: cout << "Start"; break;
    case 2: cout << "Stop"; break;
    default: cout << "Invalid";
}
```

---

# 2️⃣ Iteration (Looping) Statements

Used to **repeat a block of code** multiple times.

---

## ✔ `for` Loop
Used when the number of iterations is known.

### Example:
```cpp
for (int i = 1; i <= 5; i++) {
    cout << i << " ";
}
```

---

## ✔ `while` Loop
Used when the number of iterations is unknown.

### Example:
```cpp
int i = 1;
while (i <= 5) {
    cout << i << " ";
    i++;
}
```

---

## ✔ `do-while` Loop
Executes at least once, even if the condition is false.

### Example:
```cpp
int i = 1;
do {
    cout << i << " ";
    i++;
} while (i <= 5);
```

---

# 3️⃣ Jump Statements

Used to change the normal flow of execution.

---

## ✔ `break`
Exits a loop or switch immediately.

### Example:
```cpp
for (int i = 1; i <= 10; i++) {
    if (i == 5) break;
    cout << i << " ";
}
```

---

## ✔ `continue`
Skips the current iteration and moves to the next.

### Example:
```cpp
for (int i = 1; i <= 5; i++) {
    if (i == 3) continue;
    cout << i << " ";
}
```

---

## ✔ `return`
Exits from a function.

### Example:
```cpp
int sum(int a, int b) {
    return a + b;  // control returns to caller
}
```

---

# ⭐ Summary

| Type | Statements | Purpose |
|------|------------|----------|
| Selection | if, if-else, switch | Decision making |
| Iteration | for, while, do-while | Repetition |
| Jump | break, continue, return | Control program flow |

---

# 🎯 Conclusion
Control flow statements are essential for writing logical and structured programs.  
They help in decision-making, repeating tasks, and controlling how the program executes.

