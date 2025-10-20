
# Matrix Operations in Google Sheets

This guide explains how to perform matrix multiplication, matrix inversion, and related linear algebra operations directly in Google Sheets using built-in formulas.  
It is useful for students, researchers, or anyone performing matrix computations without coding.

---

## Features

- Matrix Multiplication using `MMULT`
- Matrix Inversion using `MINVERSE`
- Identity Matrix Verification
- Error Handling Tips
- Additional Functions: Transpose, Dot Product

---

## 1. Matrix Multiplication

Google Sheets supports matrix multiplication using the `MMULT` function.

### Syntax
```excel
=MMULT(array1, array2)
````

### Example

Matrix A (2×3) in cells `A1:C2`:

```
1   2   3
4   5   6
```

Matrix B (3×2) in cells `E1:F3`:

```
7   8
9  10
11 12
```

**Steps:**

1. Select a 2×2 cell range (for example, `H1:I2`)
2. Enter:

   ```excel
   =MMULT(A1:C2, E1:F3)
   ```
3. Press **Enter**

You will get the resulting 2×2 product matrix.

---

## 2. Matrix Inversion

Use the `MINVERSE` function to compute the inverse of a square matrix.

### Syntax

```excel
=MINVERSE(array)
```

### Example

Matrix A (3×3) in `A1:C3`:

```
2   5   7
6   3   4
5  -2  -3
```

**Steps:**

1. Select a 3×3 range (for example, `E1:G3`)
2. Type:

   ```excel
   =MINVERSE(A1:C3)
   ```
3. Press **Enter**

You will get the inverse matrix.

---

## 3. Verify the Inverse

To confirm the inverse, multiply the original matrix by its inverse:

```excel
=MMULT(A1:C3, E1:G3)
```

Expected result (approximately):

```
1  0  0
0  1  0
0  0  1
```

---

## Notes

* The matrix must be square to calculate an inverse.
* The matrix must be invertible (determinant not equal to zero).
* `MINVERSE` returns `#NUM!` if the matrix is not invertible.

---

## File link: 
[!sheet1](https://docs.google.com/spreadsheets/d/1WAygFIwGgWvAx1wNf_-_9Yp7nOq4THCqC-ZBcbiZiDc/edit?usp=sharing)

---

* Use `=TRANSPOSE(range)` to transpose a matrix.
* Use `=MMULT(TRANSPOSE(A1:A3), B1:B3)` to compute a dot product.

---


