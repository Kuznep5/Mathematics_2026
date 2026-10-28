### Exercise 4. Gauss–Jordan
 
#### Solution
 
Start with the augmented matrix $[A\mid I]$:
 
$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
3 & 5 & \mid & 0 & 1 \\
\end{pmatrix}
$$
 
Step 1: $R_2\to R_2-3R_1$.
 
$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & -1 & \mid & -3 & 1 \\
\end{pmatrix}
$$
 
Step 2: $R_2\to -R_2$.
 
$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}
$$
 
Step 3: $R_1\to R_1-2R_2$.
 
$$
\begin{pmatrix}
1 & 0 & \mid & -5 & 2 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}
$$
 
Therefore
 
$$
A^{-1}=
\begin{pmatrix}
-5 & 2 \\
3 & -1 \\
\end{pmatrix}.
$$
 
**Why this works.** Every row operation is multiplication on the left by an elementary matrix $E_k$. After all steps we have $E_m\cdots E_1A=I$, and the same operations applied to $I$ give $E_m\cdots E_1I=E_m\cdots E_1$. By the definition of the inverse, $E_m\cdots E_1=A^{-1}$. So when the left block becomes $I$, the right block is $A^{-1}$.
 
Check with the formula: $\det A=5-6=-1$ and
 
$$
A^{-1}=
\frac{1}{-1}
\begin{pmatrix}
5 & -2 \\
-3 & 1 \\
\end{pmatrix}
$$
 
which gives the same matrix.
