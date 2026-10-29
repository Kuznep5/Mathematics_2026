# Exercise 10. Inverse of a Diagonal Matrix
 
## Question
 
Given
 
$$
D=
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5 \\
\end{pmatrix},\qquad E=
\begin{pmatrix}
2 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 5 \\
\end{pmatrix}.
$$
 
Without using Gauss–Jordan elimination, decide which matrix is invertible. For the invertible matrix, give the inverse and check the result by multiplication.
 
## Solution
 
**Method.** The determinant of a diagonal matrix is the product of its diagonal entries. Therefore a diagonal matrix is invertible if and only if all its diagonal entries are nonzero, and in that case the inverse is the diagonal matrix of reciprocals.
 
**Step 1. The matrix $D$.** Its diagonal entries are $2$, $-3$, $5$, all nonzero:
 
$$
\det D=2\cdot(-3)\cdot5=-30\neq0.
$$
 
Hence $D$ is invertible.
 
**Step 2. The matrix $E$.** It has a zero on the diagonal:
 
$$
\det E=2\cdot0\cdot5=0.
$$
 
Hence $E$ is not invertible. This is also visible directly: the second row of $E$ is zero, so the rows are linearly dependent.
 
**Step 3. The inverse of $D$.** Replace each diagonal entry by its reciprocal:
 
$$
D^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5} \\
\end{pmatrix}.
$$
 
**Step 4. Check by multiplication.** The product of two diagonal matrices is the diagonal matrix of the products of the corresponding diagonal entries:
 
$$
DD^{-1}=
\begin{pmatrix}
2\cdot\frac{1}{2} & 0 & 0 \\
0 & (-3)\cdot\left(-\frac{1}{3}\right) & 0 \\
0 & 0 & 5\cdot\frac{1}{5} \\
\end{pmatrix}
$$
 
Hence
 
$$
DD^{-1}=
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{pmatrix}
=I.
$$
 
**Conclusion.** The matrix $D$ is invertible with the inverse shown above, and $E$ is not invertible.
