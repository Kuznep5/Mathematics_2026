# Exercise 7. Inverse of a Product
 
## Question
 
For
 
$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
2 & 0 \\
0 & 3 \\
\end{pmatrix}
$$
 
compute $(AB)^{-1}$ and $B^{-1}A^{-1}$. Check that the results are the same and explain the meaning of the reversed order.
 
## Solution
 
**Method.** We compute the left-hand side $(AB)^{-1}$ directly and the right-hand side $B^{-1}A^{-1}$ separately, then compare them.
 
**Part 1. Computing $(AB)^{-1}$ directly.**
 
First the product:
 
$$
AB=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 3 \\
\end{pmatrix}
$$
 
The entries are $1\cdot2+1\cdot0=2$, $1\cdot0+1\cdot3=3$, $0\cdot2+1\cdot0=0$, $0\cdot0+1\cdot3=3$. Hence
 
$$
AB=
\begin{pmatrix}
2 & 3 \\
0 & 3 \\
\end{pmatrix}.
$$
 
Its determinant is $\det(AB)=2\cdot3-3\cdot0=6\neq0$, so by the $2\times2$ formula
 
$$
(AB)^{-1}=
\frac{1}{6}
\begin{pmatrix}
3 & -3 \\
0 & 2 \\
\end{pmatrix}
$$
 
Dividing each entry by $6$:
 
$$
(AB)^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3} \\
\end{pmatrix}.
$$
 
**Part 2. Computing $B^{-1}A^{-1}$.**
 
Since $\det A=1$, the formula gives
 
$$
A^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}.
$$
 
The matrix $B$ is diagonal, so its inverse is obtained by inverting the diagonal entries:
 
$$
B^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & \frac{1}{3} \\
\end{pmatrix}.
$$
 
Now multiply in the order $B^{-1}A^{-1}$:
 
$$
B^{-1}A^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & \frac{1}{3} \\
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}
$$
 
Hence
 
$$
B^{-1}A^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3} \\
\end{pmatrix}.
$$
 
**Part 3. Comparison.** The two matrices coincide, so
 
$$
(AB)^{-1}=B^{-1}A^{-1}.
$$
 
**Meaning of the reversed order.** The product $AB$ means: first apply $B$, then apply $A$. To undo two actions, the last one has to be undone first. So we first apply $A^{-1}$ and only then $B^{-1}$. This is the same as putting on socks and then shoes: to reverse it, take off the shoes first.
 
Algebraically,
 
$$
(AB)(B^{-1}A^{-1}) = A(BB^{-1})A^{-1} = AIA^{-1} = AA^{-1} = I.
$$
 
The order cannot be swapped, because in general $AB\neq BA$.
