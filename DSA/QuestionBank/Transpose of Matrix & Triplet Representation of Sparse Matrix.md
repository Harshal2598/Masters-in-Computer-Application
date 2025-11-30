#Explain the Transpose of Matrix with example.
0.2Explain the Triplet representation of Sparse
Matrix

# 📘 Transpose of Matrix & Triplet Representation of Sparse Matrix

---

# 1️⃣ Transpose of a Matrix

## 📌 Definition
The **transpose of a matrix** is obtained by **interchanging its rows and columns**.

If a matrix **A** becomes **Aᵀ** after transpose, then:

A[i][j] → Aᵀ[j][i]

yaml
Copy code

---

## 📌 Example

### Original Matrix A (3×2):

1 2
3 4
5 6

shell
Copy code

### Transpose Aᵀ (2×3):

1 3 5
2 4 6

yaml
Copy code

✔ Row 1 becomes Column 1  
✔ Row 2 becomes Column 2  
✔ Row 3 becomes Column 3  

---

## ✔ C++ Code Example (Simple)

```cpp
for(int i=0; i<rows; i++){
    for(int j=0; j<cols; j++){
        B[j][i] = A[i][j];
    }
}
2️⃣ Triplet Representation of Sparse Matrix
📌 What is a Sparse Matrix?
A sparse matrix is a matrix that contains mostly zero values.
Instead of storing all elements, we store only the non-zero elements.

This saves memory.

📦 Triplet Representation (3-Tuple Form)
A sparse matrix is represented as:

sql
Copy code
Row | Column | Value
The first row stores:

scss
Copy code
(total_rows, total_columns, number_of_nonzero_elements)
📌 Example Sparse Matrix
Copy code
0   0   5
0   8   0
0   0   3
Matrix size = 3 × 3
Non-zero elements = 3

📌 Triplet Representation
Row	Col	Value
3	3	3
0	2	5
1	1	8
2	2	3

✔ Why Triplet Representation?
Saves storage

Efficient for matrix operations

Useful for huge matrices (like graphs, scientific computing)

✔ C++ Structure for Triplet
cpp
Copy code
struct Triplet {
    int row;
    int col;
    int value;
};
📝 Short Exam Answer
Transpose of Matrix:
Obtained by interchanging rows and columns. Example:

css
Copy code
[1 2; 3 4] → [1 3; 2 4]
Triplet Representation of Sparse Matrix:
Stores only non-zero elements in the form (row, column, value).
First row stores matrix size and total non-zero elements.

yaml
Copy code
