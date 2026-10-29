# Exercise 1. Determinant of a 2×2 Matrix
 
## Question
 
Compute
 
$$
\det
\begin{pmatrix}
3 & -2 \\
5 & 4 \\
\end{pmatrix},
\qquad
\det
\begin{pmatrix}
1 & 7 \\
2 & 14 \\
\end{pmatrix}.
$$
 
Which matrix is invertible? Justify your answer.
 
## Solution
 
### Given
 
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
 
### Find
 
The values $\det A_1$ and $\det A_2$, and decide which matrix is invertible.
 
### Method and steps
 
*Step 1. Recall the formula.* For a $2\times2$ matrix, the determinant is the product of the main diagonal minus the product of the anti-diagonal:
 
$$
\det
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}
= ad-bc.
$$
 
*Step 2. Compute $\det A_1$.* Here $a=3$, $b=-2$, $c=5$, $d=4$. Therefore
 
$$
\det A_1 = 3\cdot 4-(-2)\cdot 5 = 12+10 = 22.
$$
 
*Step 3. Compute $\det A_2$.* Here $a=1$, $b=7$, $c=2$, $d=14$. Therefore
 
$$
\det A_2 = 1\cdot 14-7\cdot 2 = 14-14 = 0.
$$
 
*Step 4. Use the invertibility criterion.* A square matrix is invertible exactly when its determinant is nonzero. Since $\det A_1=22\neq 0$, the matrix $A_1$ is invertible. Since $\det A_2=0$, the matrix $A_2$ is not invertible.
 
*Step 5. Interpret the result.* The second row of $A_2$ is twice the first row, so the rows are linearly dependent. Geometrically, $A_2$ collapses the plane onto a line, and this cannot be undone.
 
### Answer
 
$\det A_1=22$ and $\det A_2=0$. Only $A_1$ is invertible.
