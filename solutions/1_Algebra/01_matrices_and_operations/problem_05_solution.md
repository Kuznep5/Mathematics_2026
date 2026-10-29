# Exercise 5. Matrix Times Vector

## Question

Let

$$
A=
\begin{pmatrix}
2 & -1 \\
1 & 3 \\
\end{pmatrix},\qquad x=
\begin{pmatrix}
4 \\
2 \\
\end{pmatrix}.
$$

Compute $Ax$. Then express $Ax$ as a linear combination of the columns of $A$, with coefficients coming from the vector $x$.

## Solution

**Computation row by column.** Each row of $A$ is multiplied by the vector $x$, and the results are written from top to bottom:

$$
Ax=
\begin{pmatrix}
2\cdot4+(-1)\cdot2 \\
1\cdot4+3\cdot2 \\
\end{pmatrix}=
\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}.
$$

**Linear combination of the columns.** The entries of $x$ are the coefficients: the first column of $A$ is multiplied by $4$ and the second column by $2$, and the results are added:

$$
Ax=4
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}+2
\begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}=
\begin{pmatrix}
8 \\
4 \\
\end{pmatrix}+
\begin{pmatrix}
-2 \\
6 \\
\end{pmatrix}=
\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}.
$$

**Verification.** Both methods give the same vector $(6,10)^T$. The columns of $A$ act as two basic steps, and the vector $x$ says how many steps of each kind are taken.
