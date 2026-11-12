### Exercise 2. Gaussian Elimination — One Solution
 
**Problem.** Solve
 
$$
\begin{cases}
x+y+z=6, \\
2x-y+z=3, \\
x+2y-z=2.
\end{cases}
$$
 
**Solution.** The augmented matrix is
 
$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
2 & -1 & 1 & \mid & 3 \\
1 & 2 & -1 & \mid & 2 \\
\end{pmatrix}
$$
 
Step 1: $R_2\leftarrow R_2-2R_1$ and $R_3\leftarrow R_3-R_1$.
 
$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & -3 & -1 & \mid & -9 \\
0 & 1 & -2 & \mid & -4 \\
\end{pmatrix}
$$
 
Step 2: interchange $R_2$ and $R_3$.
 
$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & 1 & -2 & \mid & -4 \\
0 & -3 & -1 & \mid & -9 \\
\end{pmatrix}
$$
 
Step 3: $R_3\leftarrow R_3+3R_2$.
 
$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & 1 & -2 & \mid & -4 \\
0 & 0 & -7 & \mid & -21 \\
\end{pmatrix}
$$
 
Back substitution:
 
$$
\begin{aligned}
-7z &= -21 \quad\Rightarrow\quad z=3, \\
y-2z &= -4 \quad\Rightarrow\quad y=-4+6=2, \\
x+y+z &= 6 \quad\Rightarrow\quad x=6-2-3=1.
\end{aligned}
$$
 
**Check.**
 
$$
\begin{aligned}
1+2+3 &= 6, \\
2\cdot1-2+3 &= 3, \\
1+2\cdot2-3 &= 2.
\end{aligned}
$$
 
All three equations hold.
 
**Answer.** $(x,y,z)=(1,2,3)$.
 
---
