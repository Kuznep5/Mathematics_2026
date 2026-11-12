### Exercise 8. Two Systems with the Same Coefficient Matrix
 
**Problem.** Solve
 
$$
\begin{cases}
2x+y=5, \\
x-y=1,
\end{cases}
\qquad
\begin{cases}
2x+y=1, \\
x-y=4.
\end{cases}
$$
 
**System 1.**
 
$$
\begin{pmatrix}
2 & 1 & \mid & 5 \\
1 & -1 & \mid & 1 \\
\end{pmatrix}
$$
 
Apply $R_2\leftarrow 2R_2-R_1$:
 
$$
\begin{pmatrix}
2 & 1 & \mid & 5 \\
0 & -3 & \mid & -3 \\
\end{pmatrix}
$$
 
Hence $y=1$ and $2x=5-1=4$, so $x=2$.
 
**System 2.**
 
$$
\begin{pmatrix}
2 & 1 & \mid & 1 \\
1 & -1 & \mid & 4 \\
\end{pmatrix}
$$
 
Apply the same operation $R_2\leftarrow 2R_2-R_1$:
 
$$
\begin{pmatrix}
2 & 1 & \mid & 1 \\
0 & -3 & \mid & 7 \\
\end{pmatrix}
$$
 
Hence $y=-\tfrac73$ and $2x=1-y=\tfrac{10}{3}$, so $x=\tfrac53$.
 
**Check.** System 1: $2\cdot2+1=5$, $2-1=1$. System 2: $\tfrac{10}{3}-\tfrac73=1$, $\tfrac53+\tfrac73=4$.
 
**Comparison.** The row operations and the coefficient part of the matrix (the first two columns, with rows $2,1$ and $0,-3$) are identical in both cases. Only the last column changes. The operations are chosen using the coefficients alone, and the right-hand side is just transformed by the same operations.
 
**Answer.** System 1: $(2,1)$. System 2: $\left(\tfrac53,\,-\tfrac73\right)$.
 
---
