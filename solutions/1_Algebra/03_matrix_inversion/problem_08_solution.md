# Exercise 8. Inverse of a Transformation
 
## Question
 
The matrix
 
$$
S=
\begin{pmatrix}
2 & 0 \\
0 & \frac12 \\
\end{pmatrix}
$$
 
describes a scaling of the plane. Find $S^{-1}$ and explain geometrically what the inverse transformation does. Check the action of the pair $S,S^{-1}$ on one simple vector.
 
## Solution
 
**Method.** The matrix $S$ is diagonal, and the inverse of an invertible diagonal matrix is obtained by replacing each diagonal entry with its reciprocal.
 
**Step 1. The inverse.** The determinant is $\det S=2\cdot\frac12=1\neq0$, so $S^{-1}$ exists, and
 
$$
S^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2 \\
\end{pmatrix}.
$$
 
**Step 2. Geometric meaning.** The transformation $S$ stretches the plane by a factor of $2$ along the $x$-axis and shrinks it by a factor of $\frac12$ along the $y$-axis. The inverse transformation $S^{-1}$ does the opposite: it shrinks by a factor of $\frac12$ along the $x$-axis and stretches by a factor of $2$ along the $y$-axis. Every point is therefore returned to its original position, which means that $S^{-1}$ undoes the action of $S$. Since $\det S=1$, areas are preserved by both transformations.
 
**Step 3. Check on a vector.** Take $v=(1,\ 1)^T$. First apply $S$:
 
$$
Sv=
\begin{pmatrix}
2 & 0 \\
0 & \frac{1}{2} \\
\end{pmatrix}
\begin{pmatrix}
1 \\
1 \\
\end{pmatrix}
$$
 
Hence
 
$$
Sv=
\begin{pmatrix}
2 \\
\frac{1}{2} \\
\end{pmatrix}.
$$
 
Now apply $S^{-1}$ to the result:
 
$$
S^{-1}(Sv)=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2 \\
\end{pmatrix}
\begin{pmatrix}
2 \\
\frac{1}{2} \\
\end{pmatrix}
$$
 
Hence
 
$$
S^{-1}(Sv)=
\begin{pmatrix}
1 \\
1 \\
\end{pmatrix}
=v.
$$
 
The vector returns to its initial position, as expected.
