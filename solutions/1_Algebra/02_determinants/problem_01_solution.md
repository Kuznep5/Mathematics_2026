# Determinants: Solutions
 
## Basic Exercises
 
### Exercise 1. Determinant of a 2×2 Matrix
 
Let
 
$$
A_1=
\begin{pmatrix}
3 & -2 \\
5 & 4 \\
\end{pmatrix},
\qquad
A_2=
\begin{pmatrix}
1 & 7 \\
2 & 14 \\
\end{pmatrix}.
$$
 
For a $2\times2$ matrix, the determinant is given by
 
$$
\det
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}
= ad-bc.
$$
 
Hence
 
$$
\begin{aligned}
\det A_1 &= 3\cdot 4-(-2)\cdot 5 = 12+10 = 22, \\
\det A_2 &= 1\cdot 14-7\cdot 2 = 14-14 = 0.
\end{aligned}
$$
 
A square matrix is invertible exactly when its determinant is nonzero. Since $\det A_1=22\neq 0$ and $\det A_2=0$, the matrix $A_1$ is invertible and $A_2$ is not.
 
Indeed, the second row of $A_2$ equals twice the first row, so the rows are linearly dependent.
