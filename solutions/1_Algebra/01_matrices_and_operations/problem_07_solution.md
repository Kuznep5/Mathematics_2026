### Exercise 6. Transpose
 
Given
 
$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix}.
$$
 
**Transposes.** The rows become columns.
 
$$
A^T=
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6 \\
\end{pmatrix},\qquad B^T=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3 \\
\end{pmatrix}
$$
 
**Product.** $A$ is $2\times3$ and $B$ is $3\times2$, so $AB$ is $2\times2$.
 
$$
AB=
\begin{pmatrix}
1\cdot1+2\cdot2+3\cdot(-1) & 1\cdot0+2\cdot1+3\cdot3 \\
4\cdot1+5\cdot2+6\cdot(-1) & 4\cdot0+5\cdot1+6\cdot3 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 11 \\
8 & 23 \\
\end{pmatrix}
$$
 
**Verification of $(AB)^T=B^TA^T$.**
 
$$
(AB)^T=
\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}
$$
 
$$
B^TA^T=
\begin{pmatrix}
1\cdot1+2\cdot2+(-1)\cdot3 & 1\cdot4+2\cdot5+(-1)\cdot6 \\
0\cdot1+1\cdot2+3\cdot3 & 0\cdot4+1\cdot5+3\cdot6 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}
$$
 
The two matrices are equal. The order of the factors is reversed under transposition. The product $A^TB^T$ in the original order would be a $3\times3$ matrix, so it cannot be equal to the $2\times2$ matrix $(AB)^T$.
