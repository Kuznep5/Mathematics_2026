### Exercise 6. Solving a System Using the Inverse
 
#### Solution
 
The determinant is $\det A=2\cdot3-1\cdot1=5$, so
 
$$
A^{-1}=
\frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}.
$$
 
Then
 
$$
x=A^{-1}b=
\frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}
$$
 
Hence
 
$$
x=
\frac{1}{5}
\begin{pmatrix}
15-7 \\
-5+14 \\
\end{pmatrix}=
\begin{pmatrix}
\frac{8}{5} \\
\frac{9}{5} \\
\end{pmatrix}.
$$
 
Check by substitution:
 
$$
Ax=
\begin{pmatrix}
2\cdot\frac{8}{5}+\frac{9}{5} \\
\frac{8}{5}+3\cdot\frac{9}{5} \\
\end{pmatrix}
$$
 
Hence
 
$$
Ax=
\begin{pmatrix}
\frac{25}{5} \\
\frac{35}{5} \\
\end{pmatrix}=
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}
=b.
$$
