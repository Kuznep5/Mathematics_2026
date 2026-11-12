### Exercise 4. Infinitely Many Solutions
 
**Problem.** Solve
 
$$
\begin{cases}
x+y+z=2, \\
2x+2y+2z=4, \\
x-y+z=0.
\end{cases}
$$
 
**Solution.**
 
$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
2 & 2 & 2 & \mid & 4 \\
1 & -1 & 1 & \mid & 0 \\
\end{pmatrix}
$$
 
Apply $R_2\leftarrow R_2-2R_1$ and $R_3\leftarrow R_3-R_1$:
 
$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & 0 & 0 & \mid & 0 \\
0 & -2 & 0 & \mid & -2 \\
\end{pmatrix}
$$
 
Interchange $R_2$ and $R_3$ and divide the new $R_2$ by $-2$:
 
$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & 1 & 0 & \mid & 1 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$
 
There are two nonzero rows and three unknowns, so one variable is free. The pivots are in columns of $x$ and $y$, hence $z$ is free. Put $z=t$. Then $y=1$ and $x=2-y-z=1-t$.
 
**Check for $t=2$.** The point is $(-1,1,2)$:
 
$$
\begin{aligned}
-1+1+2 &= 2, \\
2(-1)+2\cdot1+2\cdot2 &= 4, \\
-1-1+2 &= 0.
\end{aligned}
$$
 
**Answer.** $(x,y,z)=(1-t,\;1,\;t)$, $t\in\mathbb{R}$.
 
---
