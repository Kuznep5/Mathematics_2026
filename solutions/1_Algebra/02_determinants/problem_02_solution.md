# Exercise 2. Determinant of a 3×3 Matrix

## Question

For

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
2 & 1 & 5 \\
\end{pmatrix}
$$

compute $\det A$ using Sarrus' rule. Then perform one simple check using a chosen property of the determinant.

## Solution

### Given

The matrix $A$ from the Question, of size $3\times3$.

### Find

The value $\det A$ by Sarrus' rule, and an independent check of the result.

### Method and steps

*Step 1. Recall Sarrus' rule.* For a $3\times3$ matrix with entries $a_{ij}$ (row $i$, column $j$):

$$
\det A = (a_{11}a_{22}a_{33}+a_{12}a_{23}a_{31}+a_{13}a_{21}a_{32})-(a_{13}a_{22}a_{31}+a_{11}a_{23}a_{32}+a_{12}a_{21}a_{33}).
$$

The first group consists of the main diagonal and the two parallel "wrapped" diagonals. The second group consists of the anti-diagonal and its two parallel "wrapped" diagonals. This rule works only for $3\times3$ matrices.

*Step 2. Compute the first group (plus terms).*

$$
\begin{aligned}
a_{11}a_{22}a_{33} &= 1\cdot 3\cdot 5 = 15, \\
a_{12}a_{23}a_{31} &= 2\cdot 4\cdot 2 = 16, \\
a_{13}a_{21}a_{32} &= (-1)\cdot 0\cdot 1 = 0.
\end{aligned}
$$

The sum is $15+16+0=31$.

*Step 3. Compute the second group (minus terms).*

$$
\begin{aligned}
a_{13}a_{22}a_{31} &= (-1)\cdot 3\cdot 2 = -6, \\
a_{11}a_{23}a_{32} &= 1\cdot 4\cdot 1 = 4, \\
a_{12}a_{21}a_{33} &= 2\cdot 0\cdot 5 = 0.
\end{aligned}
$$

The sum is $-6+4+0=-2$.

*Step 4. Subtract.*

$$
\det A = 31-(-2) = 33.
$$

*Step 5. Check using a property.* Adding a multiple of one row to another row does not change the determinant. Replace $R_3$ by $R_3-2R_1$. The new third row is $(2,1,5)-2(1,2,-1)=(0,-3,7)$, so

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & -3 & 7 \\
\end{pmatrix}.
$$

Expanding along the first column, only the entry $1$ is nonzero:

$$
\det A = 1\cdot\bigl(3\cdot 7-4\cdot(-3)\bigr) = 21+12 = 33.
$$

Both methods give the same value.

### Answer

$\det A=33$.
