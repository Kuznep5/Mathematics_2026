### Exercise 3. Inconsistent System
 
**Problem.** Solve or show that the system is inconsistent:
 
$$
\begin{cases}
x+2y=3, \\
2x+4y=7.
\end{cases}
$$
 
**Solution.**
 
$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
2 & 4 & \mid & 7 \\
\end{pmatrix}
$$
 
Apply $R_2\leftarrow R_2-2R_1$:
 
$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
0 & 0 & \mid & 1 \\
\end{pmatrix}
$$
 
The second row means $0\cdot x+0\cdot y=1$, that is $0=1$. This is a contradiction.
 
Interpretation: the left side of the second equation is exactly twice the left side of the first. If $x+2y=3$, then $2x+4y$ must equal $6$, not $7$. Geometrically, the lines $x+2y=3$ and $2x+4y=7$ are parallel and distinct.
 
**Answer.** The system is inconsistent; there is no solution.
 
---
