### Exercise 5. Row Operations
 
$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2 \\
\end{pmatrix}
$$
 
**Step 1.** $R_2\to R_2-2R_1$. This operation does not change the determinant.
 
$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
-1 & 4 & 2 \\
\end{pmatrix}
$$
 
**Step 2.** $R_3\to R_3+R_1$. This operation does not change the determinant.
 
$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 6 & 5 \\
\end{pmatrix}
$$
 
**Step 3.** $R_3\to R_3+2R_2$. This operation does not change the determinant.
 
$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 0 & -7 \\
\end{pmatrix}
$$
 
The final matrix is upper triangular, and no row swaps or row scalings were used, so
 
$$
\det A = 1\cdot(-3)\cdot(-7) = 21.
$$
