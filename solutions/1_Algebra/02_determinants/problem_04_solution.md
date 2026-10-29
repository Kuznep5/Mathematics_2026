# Exercise 4. Triangular Matrix

## Question

Without expanding the determinant, compute

$$
\det
\begin{pmatrix}
2 & 4 & 1 \\
0 & -3 & 5 \\
0 & 0 & 7 \\
\end{pmatrix}.
$$

State the rule for an arbitrary triangular matrix and explain it using this example.

## Solution

### Given

An upper triangular $3\times3$ matrix (all entries below the main diagonal are zero).

### Find

The determinant, and the general rule for triangular matrices with an explanation.

### Method and steps

*Step 1. Identify the structure.* All entries below the main diagonal are zero, so the matrix is upper triangular. The diagonal entries are $2$, $-3$ and $7$.

*Step 2. Apply the rule.* The determinant of a triangular matrix is the product of its diagonal entries:

$$
\det = 2\cdot(-3)\cdot 7 = -42.
$$

*Step 3. State the general rule.* For any upper or lower triangular matrix of size $n\times n$ with diagonal entries $d_1,\dots,d_n$,

$$
\det = d_1d_2\cdots d_n.
$$

*Step 4. Explain the rule on this example.* In the first column, only the entry $2$ is nonzero. Expanding along this column leaves one term:

$$
\det = 2\cdot\det
\begin{pmatrix}
-3 & 5 \\
0 & 7 \\
\end{pmatrix}.
$$

The remaining $2\times2$ matrix is again triangular. Its determinant is $-3\cdot7-5\cdot0=-21$, so

$$
\det = 2\cdot(-21) = -42.
$$

Each expansion removes one row and one column and leaves a smaller triangular matrix, so the same argument works for any size $n$. For a lower triangular matrix, the argument is the same with expansion along the first row.

### Answer

$\det=-42$. The determinant of a triangular matrix equals the product of its diagonal entries.
