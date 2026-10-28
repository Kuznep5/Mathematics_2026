### Exercise 2. Formula for a 2×2 Matrix
 
#### Solution
 
For a matrix
 
$$
A=
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}
$$
 
the inverse is given by
 
$$
A^{-1}=
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a \\
\end{pmatrix}
$$
 
provided that $ad-bc\neq0$.
 
Here the determinant is
 
$$
\det A = 3\cdot4-2\cdot5 = 2 \neq 0,
$$
 
so the inverse exists. Applying the formula:
 
$$
A^{-1}=
\frac{1}{2}
\begin{pmatrix}
4 & -2 \\
-5 & 3 \\
\end{pmatrix}
$$
 
Therefore
 
$$
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2} \\
\end{pmatrix}.
$$
 
Check by computing $AA^{-1}$:
 
$$
AA^{-1}=
\begin{pmatrix}
3\cdot2+2\cdot\left(-\frac{5}{2}\right) & 3\cdot(-1)+2\cdot\frac{3}{2} \\
5\cdot2+4\cdot\left(-\frac{5}{2}\right) & 5\cdot(-1)+4\cdot\frac{3}{2} \\
\end{pmatrix}
$$
 
Hence
 
$$
AA^{-1}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I.
$$
