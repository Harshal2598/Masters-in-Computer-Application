#Q. “What is a sparse matrix? How is it represented in triplet format?”

# 📘 Sparse Matrix & Triplet Representation

## 1️⃣ What is a Sparse Matrix?

A **sparse matrix** is a matrix in which **most of the elements are zero**.

### ✔ Key Points
- Contains very few non-zero elements  
- Storing all elements wastes memory  
- Efficient storage formats are used (Triplet, CSR, etc.)

### ✔ Example of Sparse Matrix


0 0 5
0 8 0
0 0 3


Total elements = 9  
Non-zero = 3 → Sparse Matrix ✔

---

# 2️⃣ Triplet Representation of Sparse Matrix

The **Triplet (3-tuple) representation** stores only the **non-zero elements** of the matrix.

It uses a 2D table with **three columns**:



Row | Column | Value


### ✔ First Row Stores Metadata


(total_rows, total_columns, number_of_nonzero_elements)


---

## 📌 Example Sparse Matrix

Matrix:


0 0 5
0 8 0
0 0 3


Rows = 3  
Columns = 3  
Non-zero elements = 3  

---

## 📌 Triplet Representation

| Row | Col | Value |
|-----|------|--------|
| 3   | 3    | 3      |  ← metadata: (rows, cols, non-zero count)
| 0   | 2    | 5      |
| 1   | 1    | 8      |
| 2   | 2    | 3      |

### ✔ Explanation
- First row: matrix info  
- Next rows: each non-zero value with its row, column, and data

---

## ✔ Advantages of Triplet Format
- Saves memory  
- Easy to traverse  
- Useful for matrix operations  
- Efficient for large sparse matrices  

---

# 📝 Short Exam Answer

A **sparse matrix** is a matrix that contains mostly zero values.  
To save space, it is stored in **Triplet format** which uses three columns:



(Row, Column, Value)


The first row stores:


(total_rows, total_columns, number_of_nonzero_elements)


Each subsequent row stores the position and value of a non-zero element.
