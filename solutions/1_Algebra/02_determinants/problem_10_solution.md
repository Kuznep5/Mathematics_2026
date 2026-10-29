# Exercise 10. Detecting Dependence

## Question

Without carrying out a full determinant calculation, explain why

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5 \\
\end{pmatrix}=0.
$$

Identify a specific dependence between the rows and connect it with noninvertibility of the matrix.

## Solution

### Given

The $3\times3$ matrix from the Question, with rows $R_1=(1,2,3)$, $R_2=(2,4,6)$ and $R_3=(0,1,5)$.

### Find

An explanation of why the determinant is zero, a specific dependence between the rows, and the link to invertibility.

### Method and steps

*Step 1. Compare the rows.* The second row is exactly twice the first row:

$$
R_2 = 2R_1.
$$

*Step 2. Apply a row operation.* Replace $R_2$ by $R_2-2R_1$. This operation does not change the determinant, and it produces a zero row:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & 0 \\
0 & 1 & 5 \\
\end{pmatrix}.
$$

*Step 3. Conclude that the determinant is zero.* A matrix with a zero row has determinant $0$. Indeed, multiplying the zero row by any number $c$ leaves the matrix unchanged, but multiplies the determinant by $c$. Taking $c=2$ gives $\det=2\det$, so $\det=0$.

*Step 4. State the dependence.* The relation $2R_1-R_2=0$ is a nontrivial linear dependence between the rows.

*Step 5. Connect with invertibility.* Linearly dependent rows mean that the matrix does not have full rank, so it is not invertible. This agrees with the criterion that a matrix is invertible exactly when its determinant is nonzero.

### Answer

$\det=0$, because $R_2=2R_1$, that is, $2R_1-R_2=0$. The rows are linearly dependent, so the matrix is not invertible.
