# Exercise 2. Formula for a 2×2 Matrix
 
## Question
 
Find the inverse of
 
$$
A=
\begin{pmatrix}
3 & 2 \\
5 & 4 \\
\end{pmatrix}
$$
 
using the formula for a $2\times2$ matrix. At the end, check the result by computing one product with $A$.
 
## Solution
 
**Method.** For a $2\times2$ matrix there is an explicit formula. If
 
$$
A=
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}
$$
 
and $ad-bc\neq0$, then
 
$$
A^{-1}=
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a \\
\end{pmatrix}.
$$
 
In words: swap the diagonal entries, change the signs of the off-diagonal entries, and divide by the determinant. The condition $ad-bc\neq0$ is necessary, because the formula divides by the determinant.
 
**Step 1. The determinant.** Here $a=3$, $b=2$, $c=5$, $d=4$, so
 
$$
\det A = 3\cdot4-2\cdot5 = 12-10 = 2 \neq 0.
$$
 
The determinant is nonzero, so the inverse exists.
 
**Step 2. Apply the formula.**
 
$$
A^{-1}=
\frac{1}{2}
\begin{pmatrix}
4 & -2 \\
-5 & 3 \\
\end{pmatrix}
$$
 
Multiplying every entry by $\frac12$ gives
 
$$
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2} \\
\end{pmatrix}.
$$
 
**Step 3. Check.** By the definition of the inverse, the product $AA^{-1}$ must be $I$:
 
$$
AA^{-1}=
\begin{pmatrix}
3\cdot2+2\cdot\left(-\frac{5}{2}\right) & 3\cdot(-1)+2\cdot\frac{3}{2} \\
5\cdot2+4\cdot\left(-\frac{5}{2}\right) & 5\cdot(-1)+4\cdot\frac{3}{2} \\
\end{pmatrix}
$$
 
Simplifying the entries:
 
$$
AA^{-1}=
\begin{pmatrix}
6-5 & -3+3 \\
10-10 & -5+6 \\
\end{pmatrix}
$$
 
Hence
 
$$
AA^{-1}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I.
$$
 
The check succeeds, so the inverse is correct.
