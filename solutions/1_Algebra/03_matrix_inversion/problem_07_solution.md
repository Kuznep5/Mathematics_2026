### Exercise 7. Inverse of a Product
 
#### Solution
 
First compute the product:
 
$$
AB=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 3 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 3 \\
0 & 3 \\
\end{pmatrix}.
$$
 
Its determinant is $\det(AB)=6$, so by the $2\times2$ formula
 
$$
(AB)^{-1}=
\frac{1}{6}
\begin{pmatrix}
3 & -3 \\
0 & 2 \\
\end{pmatrix}
$$
 
Hence
 
$$
(AB)^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3} \\
\end{pmatrix}.
$$
 
Now the individual inverses:
 
$$
A^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix},\qquad
B^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & \frac{1}{3} \\
\end{pmatrix}.
$$
 
Then
 
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
 
The two results coincide, so $(AB)^{-1}=B^{-1}A^{-1}$.
 
**Meaning of the reversed order.** The product $AB$ applies $B$ first and then $A$. To undo this, the last step must be undone first, that is $A^{-1}$, and then $B^{-1}$. Algebraically:
 
$$
(AB)(B^{-1}A^{-1}) = A(BB^{-1})A^{-1} = AA^{-1} = I.
$$
 
Also, $AB\neq BA$ in general, so the order cannot be swapped.
