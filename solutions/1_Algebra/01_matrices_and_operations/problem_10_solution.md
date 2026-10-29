# Exercise 10. Columns of a Matrix Product

## Question

Given

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1 \\
\end{pmatrix}.
$$

Denote the columns of $B$ by $b_1,b_2$.

1. Compute $Ab_1$ and $Ab_2$.
2. Compute the matrix $AB$.
3. Compare the results and explain why the columns of $AB$ are exactly the vectors $Ab_1$ and $Ab_2$.

## Solution

The columns of $B$ are

$$
b_1=
\begin{pmatrix}
1 \\
-1 \\
3 \\
\end{pmatrix},\qquad b_2=
\begin{pmatrix}
2 \\
0 \\
1 \\
\end{pmatrix}.
$$

**Part 1. Matrix-vector products.** Each row of $A$ is multiplied by the given column, and the results are written from top to bottom:

$$
Ab_1=
\begin{pmatrix}
1\cdot1+2\cdot(-1)+0\cdot3 \\
0\cdot1+1\cdot(-1)+1\cdot3 \\
\end{pmatrix}=
\begin{pmatrix}
-1 \\
2 \\
\end{pmatrix},
$$

$$
Ab_2=
\begin{pmatrix}
1\cdot2+2\cdot0+0\cdot1 \\
0\cdot2+1\cdot0+1\cdot1 \\
\end{pmatrix}=
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}.
$$

**Part 2. The product $AB$.** The sizes $(2\times3)(3\times2)$ are compatible, so $AB$ is a $2\times2$ matrix. Each entry is a row of $A$ times a column of $B$:

$$
AB=
\begin{pmatrix}
1\cdot1+2\cdot(-1)+0\cdot3 & 1\cdot2+2\cdot0+0\cdot1 \\
0\cdot1+1\cdot(-1)+1\cdot3 & 0\cdot2+1\cdot0+1\cdot1 \\
\end{pmatrix}=
\begin{pmatrix}
-1 & 2 \\
2 & 1 \\
\end{pmatrix}.
$$

**Part 3. Comparison and explanation.** The first column of $AB$ is $(-1,2)^T=Ab_1$ and the second column is $(2,1)^T=Ab_2$.

This is not a coincidence. The entry in row $i$ and column $j$ of $AB$ is (row $i$ of $A$) times (column $j$ of $B$). Therefore the whole column $j$ of $AB$ consists of the products of all rows of $A$ with the same column $b_j$, and this is exactly the vector $Ab_j$. So $AB$ is obtained by applying $A$ to every column of $B$ separately:

$$
AB=
\begin{pmatrix}
Ab_1 & Ab_2 \\
\end{pmatrix}.
$$
