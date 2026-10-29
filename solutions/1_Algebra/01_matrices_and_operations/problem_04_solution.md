# Exercise 4. Matrix Multiplication and Noncommutativity

## Question

For

$$
A=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix}
$$

compute $AB$ and $BA$. Is $AB=BA$? Use this example to explain what noncommutativity of matrix multiplication means.

## Solution

The entry $(i,j)$ of a product is obtained by multiplying row $i$ of the first matrix by column $j$ of the second matrix: the entries are multiplied in pairs and the products are added.

For $AB$, the rows are taken from $A$ and the columns from $B$:

$$
AB=
\begin{pmatrix}
1\cdot2+2\cdot3 & 1\cdot0+2\cdot1 \\
0\cdot2+1\cdot3 & 0\cdot0+1\cdot1 \\
\end{pmatrix}=
\begin{pmatrix}
8 & 2 \\
3 & 1 \\
\end{pmatrix}.
$$

For $BA$, the roles are exchanged: the rows are taken from $B$ and the columns from $A$:

$$
BA=
\begin{pmatrix}
2\cdot1+0\cdot0 & 2\cdot2+0\cdot1 \\
3\cdot1+1\cdot0 & 3\cdot2+1\cdot1 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 4 \\
3 & 7 \\
\end{pmatrix}.
$$

**Comparison.** $AB\neq BA$, for example the entries in position $(1,1)$ are $8$ and $2$.

**Noncommutativity.** For numbers $ab=ba$ always holds, but for matrices the order of the factors in general changes the result. The product $AB$ means "apply $B$ first, then $A$", while $BA$ means the opposite, and different orders of operations give different results.

**Verification.** Both products are $2\times2$ matrices, as predicted by the size rule, and every entry was recomputed row by column.
