### Exercise 8. Inverse of a Transformation
 
#### Solution
 
For a diagonal matrix the inverse is obtained by inverting the diagonal entries:
 
$$
S^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2 \\
\end{pmatrix}.
$$
 
**Geometric meaning.** $S$ stretches the plane by a factor of $2$ along the $x$-axis and shrinks it by a factor of $\frac{1}{2}$ along the $y$-axis. The inverse $S^{-1}$ does the opposite: it shrinks by a factor of $\frac{1}{2}$ along the $x$-axis and stretches by a factor of $2$ along the $y$-axis, restoring every point to its original position. Since $\det S=1$, areas are preserved by both maps.
 
**Check on a vector.** Take $v=(1,\ 1)^T$. Then
 
$$
Sv=
\begin{pmatrix}
2 & 0 \\
0 & \frac{1}{2} \\
\end{pmatrix}
\begin{pmatrix}
1 \\
1 \\
\end{pmatrix}=
\begin{pmatrix}
2 \\
\frac{1}{2} \\
\end{pmatrix}
$$
 
and
 
$$
S^{-1}(Sv)=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2 \\
\end{pmatrix}
\begin{pmatrix}
2 \\
\frac{1}{2} \\
\end{pmatrix}=
\begin{pmatrix}
1 \\
1 \\
\end{pmatrix}
=v.
$$
