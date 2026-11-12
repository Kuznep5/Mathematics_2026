### Exercise 6. A System with a Parameter — Which Cases Actually Occur?
 
**Problem.** Analyze, depending on $a$, the system
 
$$
\begin{cases}
x+y=2, \\
ax+ay=4.
\end{cases}
$$
 
**Solution.**
 
$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
a & a & \mid & 4 \\
\end{pmatrix}
$$
 
Apply $R_2\leftarrow R_2-aR_1$:
 
$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 4-2a \\
\end{pmatrix}
$$
 
The second row reads $0=4-2a$.
 
- If $a=2$, then $0=0$. One equation remains for two unknowns: $x=2-t$, $y=t$. There are infinitely many solutions.
- If $a\neq2$, then $0=4-2a\neq0$, a contradiction. There is no solution.
Exactly one solution never occurs. The second row of the coefficient matrix is always $a$ times the first, so the elimination always produces a zero row in the coefficient part. At most one pivot exists, while there are two unknowns, so at least one variable cannot be determined uniquely.
 
**Answer.** $a=2$: infinitely many solutions $(2-t,\,t)$; $a\neq2$: no solution; a unique solution does not occur.
 
---
