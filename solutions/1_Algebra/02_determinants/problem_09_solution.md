### Exercise 9. Area and the Determinant
 
$$
u=
\begin{pmatrix}
3 \\
1 \\
\end{pmatrix},
\qquad
v=
\begin{pmatrix}
1 \\
4 \\
\end{pmatrix}
$$
 
The area of the parallelogram spanned by $u$ and $v$ is the absolute value of the determinant of the matrix whose columns are $u$ and $v$:
 
$$
\det
\begin{pmatrix}
3 & 1 \\
1 & 4 \\
\end{pmatrix}
= 3\cdot 4-1\cdot 1 = 11.
$$
 
Hence the area is $|11|=11$.
 
**Reversing the order.** Taking $v$ first and $u$ second swaps the columns:
 
$$
\det
\begin{pmatrix}
1 & 3 \\
4 & 1 \\
\end{pmatrix}
= 1\cdot 1-3\cdot 4 = -11.
$$
 
Swapping two columns changes the sign of the determinant, so the determinant becomes $-11$. The sign encodes the orientation of the pair of vectors. The parallelogram itself is the same, so its area is still $|-11|=11$.
