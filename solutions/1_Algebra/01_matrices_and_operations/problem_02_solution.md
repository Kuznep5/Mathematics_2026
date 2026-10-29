# Exercise 2. Addition and Scalar Multiplication

## Question

For

$$
A=
\begin{pmatrix}
1 & 2 \\
-1 & 3 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
4 & -2 \\
0 & 5 \\
\end{pmatrix}
$$

compute

$$
A+B,\qquad A-B,\qquad 3A-2B.
$$

Explain why matrix addition is possible only for matrices of the same size.

## Solution

Addition, subtraction and multiplication by a number are performed entry by entry: the entry in position $(i,j)$ of the result depends only on the entries in position $(i,j)$ of the given matrices.

For the sum, the corresponding entries are added:

$$
A+B=
\begin{pmatrix}
1+4 & 2+(-2) \\
-1+0 & 3+5 \\
\end{pmatrix}=
\begin{pmatrix}
5 & 0 \\
-1 & 8 \\
\end{pmatrix}.
$$

For the difference, the corresponding entries are subtracted:

$$
A-B=
\begin{pmatrix}
1-4 & 2-(-2) \\
-1-0 & 3-5 \\
\end{pmatrix}=
\begin{pmatrix}
-3 & 4 \\
-1 & -2 \\
\end{pmatrix}.
$$

For $3A-2B$, first every entry of $A$ is multiplied by $3$ and every entry of $B$ by $2$:

$$
3A=
\begin{pmatrix}
3 & 6 \\
-3 & 9 \\
\end{pmatrix},\qquad 2B=
\begin{pmatrix}
8 & -4 \\
0 & 10 \\
\end{pmatrix}.
$$

Then the results are subtracted entry by entry:

$$
3A-2B=
\begin{pmatrix}
3-8 & 6-(-4) \\
-3-0 & 9-10 \\
\end{pmatrix}=
\begin{pmatrix}
-5 & 10 \\
-3 & -1 \\
\end{pmatrix}.
$$

**Why the sizes must agree.** Addition adds entries that occupy the same position. If the matrices have different sizes, some entry has no partner in the other matrix, so the sum is not defined.

**Verification.** The sum $(A+B)+(A-B)$ must equal $2A$. The first row gives $5+(-3)=2$ and $0+4=4$, which is the first row of $2A$. The second row gives $-1+(-1)=-2$ and $8+(-2)=6$, which is the second row of $2A$.
