### Exercise 10. Detecting Dependence
 
$$
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5 \\
\end{pmatrix}
$$
 
The second row is exactly twice the first row:
 
$$
R_2 = 2R_1.
$$
 
Applying $R_2\to R_2-2R_1$ does not change the determinant, but it produces a zero row:
 
$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & 0 \\
0 & 1 & 5 \\
\end{pmatrix}.
$$
 
A matrix with a zero row has determinant $0$ (expand along that row, or note that multiplying the zero row by any scalar leaves the matrix unchanged while multiplying the determinant by that scalar). Hence
 
$$
\det = 0.
$$
 
Because the rows are linearly dependent ($2R_1-R_2=0$), the matrix does not have full rank, so it is not invertible.
