# Exercise 9. Matrix Equation
 
## Question
 
Given
 
$$
A=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}.
$$
 
Solve the equation $AX=B$ for $X$. Before calculating, decide on which side of the equation $A^{-1}$ must be used. Then check the result by computing $AX$.
 
## Solution
 
**Step 1. On which side must $A^{-1}$ be used?** In the equation $AX=B$ the matrix $A$ stands on the left of $X$. To cancel it, we multiply both sides on the left by $A^{-1}$:
 
$$
A^{-1}(AX)=A^{-1}B.
$$
 
By associativity, $(A^{-1}A)X=IX=X$, so
 
$$
X=A^{-1}B.
$$
 
Multiplication on the right would give $AXA^{-1}=BA^{-1}$, which does not isolate $X$. Matrix multiplication is not commutative, so the side matters.
 
**Step 2. The inverse of $A$.** The determinant is $\det A=1\cdot1-2\cdot0=1\neq0$, so by the $2\times2$ formula
 
$$
A^{-1}=
\begin{pmatrix}
1 & -2 \\
0 & 1 \\
\end{pmatrix}.
$$
 
**Step 3. Compute $X=A^{-1}B$.**
 
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
 
The entries are $1\cdot3-2\cdot2=-1$, $1\cdot1-2\cdot4=-7$, $0\cdot3+1\cdot2=2$, $0\cdot1+1\cdot4=4$. Hence
 
$$
X=
\begin{pmatrix}
-1 & -7 \\
2 & 4 \\
\end{pmatrix}.
$$
 
**Step 4. Check by computing $AX$.** The product must equal $B$:
 
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
\end{pmatrix}
$$
 
and therefore
 
$$
AX=
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}
=B.
$$
 
The check succeeds, so the solution is correct.
