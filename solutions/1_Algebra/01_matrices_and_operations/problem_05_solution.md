### Exercise 5. Matrix Times Vector
 
Given
 
$$
A=
\begin{pmatrix}
2 & -1 \\
1 & 3 \\
\end{pmatrix},\qquad x=
\begin{pmatrix}
4 \\
2 \\
\end{pmatrix}.
$$
 
**Main steps (row by column).**
 
$$
Ax=
\begin{pmatrix}
2\cdot4+(-1)\cdot2 \\
1\cdot4+3\cdot2 \\
\end{pmatrix}=
\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}
$$
 
**Linear combination of the columns.** The coefficients are the entries of $x$: the first column is multiplied by $4$ and the second by $2$.
 
$$
Ax=4
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}+2
\begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}=
\begin{pmatrix}
8 \\
4 \\
\end{pmatrix}+
\begin{pmatrix}
-2 \\
6 \\
\end{pmatrix}=
\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}
$$
 
**Verification.** Both methods give the same vector $(6,10)$.
