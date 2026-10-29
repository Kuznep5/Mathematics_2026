# Exercise 1. Matrix Size and Entries

## Question

Given

$$
A=
\begin{pmatrix}
2 & -1 & 3 \\
0 & 4 & 5 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
1 & 0 \\
-2 & 3 \\
4 & 1 \\
\end{pmatrix}.
$$

1. State the sizes of matrices $A$ and $B$.
2. Read off the entries $a_{12}$, $a_{23}$, $b_{21}$, and $b_{32}$.
3. Write the second row of $A$ and the first column of $B$ as vectors.

## Solution

**Part 1.** The size of a matrix is written as (number of rows) $\times$ (number of columns). The matrix $A$ has 2 rows and 3 columns, so it is a $2\times3$ matrix. The matrix $B$ has 3 rows and 2 columns, so it is a $3\times2$ matrix.

**Part 2.** The entry $a_{ij}$ lies in row $i$ and column $j$: the first index is the row, the second is the column. Therefore

$$
a_{12}=-1,\qquad a_{23}=5,\qquad b_{21}=-2,\qquad b_{32}=1.
$$

**Part 3.** The second row of $A$ is read from left to right:

$$
\begin{pmatrix}
0 & 4 & 5 \\
\end{pmatrix}.
$$

The first column of $B$ is read from top to bottom:

$$
\begin{pmatrix}
1 \\
-2 \\
4 \\
\end{pmatrix}.
$$

**Verification.** $A$ has $2\cdot3=6$ entries and $B$ has $3\cdot2=6$ entries, which agrees with the numbers written in each matrix.
