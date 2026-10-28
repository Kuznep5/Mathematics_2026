### Exercise 10. Inverse of a Diagonal Matrix
 
#### Solution
 
A diagonal matrix is invertible if and only if all its diagonal entries are nonzero, because its determinant is the product of the diagonal entries.
 
- $D$ has diagonal entries $2,\ -3,\ 5$, all nonzero, so $\det D=-30\neq0$ and $D$ is invertible.
- $E$ has a zero on the diagonal, so $\det E=0$. Its second row is zero, so $E$ is not invertible.
The inverse of $D$ is obtained by inverting each diagonal entry:
 
$$
D^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5} \\
\end{pmatrix}.
$$
 
Check by multiplication:
 
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
