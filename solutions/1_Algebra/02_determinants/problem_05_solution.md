# Exercise 5. Row Operations

## Question

For

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2 \\
\end{pmatrix}
$$

find $\det A$ by simplifying the matrix with row operations. At each step, indicate whether and how the determinant changes.

## Solution

### Given

The matrix $A$ from the Question.

### Find

The value $\det A$ obtained by reducing $A$ to triangular form, with the effect of each step on the determinant.

### Method and steps

*Step 1. Recall the effect of row operations.*

- Swapping two rows multiplies the determinant by $-1$.
- Multiplying a row by a number $c$ multiplies the determinant by $c$.
- Adding a multiple of one row to another row does not change the determinant.

*Step 2. Clear the first column below the pivot.* Apply $R_2\to R_2-2R_1$. The determinant does not change.

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
-1 & 4 & 2 \\
\end{pmatrix}
$$

Apply $R_3\to R_3+R_1$. The determinant does not change.

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 6 & 5 \\
\end{pmatrix}
$$

*Step 3. Clear the second column below the pivot.* Apply $R_3\to R_3+2R_2$. The determinant does not change.

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 0 & -7 \\
\end{pmatrix}
$$

*Step 4. Read off the determinant.* The matrix is upper triangular. Only operations of the third type were used, so the determinant of the final matrix equals $\det A$:

$$
\det A = 1\cdot(-3)\cdot(-7) = 21.
$$

*Step 5. Check by Sarrus' rule.* The plus terms are $1\cdot1\cdot2=2$, $2\cdot0\cdot(-1)=0$ and $3\cdot2\cdot4=24$. The minus terms are $3\cdot1\cdot(-1)=-3$, $1\cdot0\cdot4=0$ and $2\cdot2\cdot2=8$. Hence

$$
\det A = (2+0+24)-(-3+0+8) = 26-5 = 21.
$$

### Answer

$\det A=21$.
