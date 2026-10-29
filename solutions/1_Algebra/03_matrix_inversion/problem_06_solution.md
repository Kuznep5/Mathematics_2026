# Exercise 6. Solving a System Using the Inverse
 
## Question
 
Solve
 
$$
Ax=b,
$$
 
where
 
$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix},\qquad b=
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix},
$$
 
using $x=A^{-1}b$. Then substitute the resulting vector back into the equation and check the result.
 
## Solution
 
**Method.** If $A$ is invertible, multiply both sides of $Ax=b$ on the left by $A^{-1}$:
 
$$
A^{-1}Ax=A^{-1}b.
$$
 
Since $A^{-1}A=I$ and $Ix=x$, we obtain
 
$$
x=A^{-1}b.
$$
 
**Step 1. The determinant.**
 
$$
\det A=2\cdot3-1\cdot1=6-1=5\neq0,
$$
 
so $A^{-1}$ exists.
 
**Step 2. The inverse.** By the $2\times2$ formula,
 
$$
A^{-1}=
\frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}.
$$
 
**Step 3. Multiply $A^{-1}$ by $b$.**
 
$$
x=A^{-1}b=
\frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}
$$
 
The first component is $3\cdot5-1\cdot7=8$ and the second is $-1\cdot5+2\cdot7=9$, so
 
$$
x=
\frac{1}{5}
\begin{pmatrix}
15-7 \\
-5+14 \\
\end{pmatrix}
$$
 
Hence
 
$$
x=
\begin{pmatrix}
\frac{8}{5} \\
\frac{9}{5} \\
\end{pmatrix}.
$$
 
**Step 4. Substitute back.** The vector $x$ is a solution if $Ax=b$:
 
$$
Ax=
\begin{pmatrix}
2\cdot\frac{8}{5}+\frac{9}{5} \\
\frac{8}{5}+3\cdot\frac{9}{5} \\
\end{pmatrix}
$$
 
Simplifying:
 
$$
Ax=
\begin{pmatrix}
\frac{25}{5} \\
\frac{35}{5} \\
\end{pmatrix}
$$
 
Hence
 
$$
Ax=
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}
=b.
$$
 
The equation holds, so the solution is $x_1=\frac85$, $x_2=\frac95$.
