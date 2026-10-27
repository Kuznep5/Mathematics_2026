### Exercise 8. Determinant of a Product
 
Let $\det A=3$ and $\det B=-5$.
 
$$
\begin{aligned}
\det(AB) &= \det A\cdot\det B = 3\cdot(-5) = -15, \\
\det(BA) &= \det B\cdot\det A = (-5)\cdot 3 = -15.
\end{aligned}
$$
 
Since $\det A=3\neq 0$, the matrix $A$ is invertible, and $\det(A^{-1})=\dfrac{1}{\det A}$. Therefore $A^{-1}B$ exists and
 
$$
\det(A^{-1}B) = \det(A^{-1})\cdot\det B = \frac{1}{3}\cdot(-5) = -\frac{5}{3}.
$$
 
**Why $\det(AB)=\det(BA)$ although usually $AB\neq BA$.** The matrices $AB$ and $BA$ may be different, but their determinants are products of the same two real numbers $\det A$ and $\det B$. Multiplication of real numbers is commutative, so the order does not matter.
