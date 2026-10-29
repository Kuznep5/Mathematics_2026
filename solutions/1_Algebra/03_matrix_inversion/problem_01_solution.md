# Exercise 1. Definition of the Inverse
 
## Question
 
For
 
$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
1 & -1 \\
-1 & 2 \\
\end{pmatrix}
$$
 
check, without using a formula, whether $B=A^{-1}$. Compute $AB$ and $BA$ and relate the result to the definition of the inverse.
 
## Solution
 
By definition, a matrix $B$ is the inverse of $A$ if and only if both products equal the identity matrix:
 
$$
AB=BA=I.
$$
 
Matrix multiplication is not commutative in general, so both orders have to be checked. Each entry of a product is the dot product of a row of the first matrix with a column of the second matrix.
 
**Step 1. The product $AB$.**
 
$$
AB=
\begin{pmatrix}
2\cdot1+1\cdot(-1) & 2\cdot(-1)+1\cdot2 \\
1\cdot1+1\cdot(-1) & 1\cdot(-1)+1\cdot2 \\
\end{pmatrix}
$$
 
Evaluating the entries:
 
$$
AB=
\begin{pmatrix}
2-1 & -2+2 \\
1-1 & -1+2 \\
\end{pmatrix}
$$
 
Hence
 
$$
AB=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I.
$$
 
**Step 2. The product $BA$.**
 
$$
BA=
\begin{pmatrix}
1\cdot2+(-1)\cdot1 & 1\cdot1+(-1)\cdot1 \\
(-1)\cdot2+2\cdot1 & (-1)\cdot1+2\cdot1 \\
\end{pmatrix}
$$
 
Evaluating the entries:
 
$$
BA=
\begin{pmatrix}
2-1 & 1-1 \\
-2+2 & -1+2 \\
\end{pmatrix}
$$
 
Hence
 
$$
BA=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I.
$$
 
**Conclusion.** Both products are equal to $I$, which is exactly the definition of the inverse. Therefore $B=A^{-1}$.
