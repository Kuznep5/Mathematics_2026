### Exercise 4. Triangular Matrix
 
$$
\begin{pmatrix}
2 & 4 & 1 \\
0 & -3 & 5 \\
0 & 0 & 7 \\
\end{pmatrix}
$$
 
This matrix is upper triangular, so its determinant is the product of the diagonal entries:
 
$$
\det = 2\cdot(-3)\cdot 7 = -42.
$$
 
**Rule.** For any triangular matrix (upper or lower), the determinant equals the product of the entries on the main diagonal.
 
**Explanation using this example.** Expanding along the first column, only the entry $2$ is nonzero, so
 
$$
\det = 2\cdot\det
\begin{pmatrix}
-3 & 5 \\
0 & 7 \\
\end{pmatrix}.
$$
 
The remaining $2\times2$ matrix is again triangular. Its determinant is $-3\cdot 7-5\cdot 0=-21$, so the full determinant is $2\cdot(-21)=-42$. The same argument works for any size.
