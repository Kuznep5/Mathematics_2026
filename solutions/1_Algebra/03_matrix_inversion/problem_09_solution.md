### Exercise 9. Matrix Equation
 
#### Solution
 
In $AX=B$ the matrix $A$ stands on the left of $X$. To cancel it, multiply both sides **on the left** by $A^{-1}$:
 
$$
A^{-1}(AX)=A^{-1}B
$$
 
so
 
$$
X=A^{-1}B.
$$
 
Multiplying on the right would give $AXA^{-1}=BA^{-1}$, which does not isolate $X$.
 
The determinant is $\det A=1$, so
 
$$
A^{-1}=
\begin{pmatrix}
1 & -2 \\
0 & 1 \\
\end{pmatrix}.
$$
 
Then
 
$$
X=
\begin{pmatrix}
1 & -2 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}
$$
 
Hence
 
$$
X=
\begin{pmatrix}
3-4 & 1-8 \\
2 & 4 \\
\end{pmatrix}=
\begin{pmatrix}
-1 & -7 \\
2 & 4 \\
\end{pmatrix}.
$$
 
Check by computing $AX$:
 
$$
AX=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
-1 & -7 \\
2 & 4 \\
\end{pmatrix}
$$
 
Hence
 
$$
AX=
\begin{pmatrix}
-1+4 & -7+8 \\
2 & 4 \\
\end{pmatrix}=
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}
=B.
$$
