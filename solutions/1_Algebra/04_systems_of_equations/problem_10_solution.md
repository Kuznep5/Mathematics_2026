### Exercise 10. A Polynomial Through Three Points
 
**Problem.** Find $p(x)=ax^2+bx+c$ through $(0,1)$, $(1,3)$, $(2,9)$.
 
**Solution.** Each point gives one equation in the unknowns $a,b,c$:
 
$$
\begin{cases}
c=1, \\
a+b+c=3, \\
4a+2b+c=9.
\end{cases}
$$
 
Augmented matrix, with columns for $a,b,c$:
 
$$
\begin{pmatrix}
0 & 0 & 1 & \mid & 1 \\
1 & 1 & 1 & \mid & 3 \\
4 & 2 & 1 & \mid & 9 \\
\end{pmatrix}
$$
 
Substituting $c=1$ gives
 
$$
\begin{cases}
a+b=2, \\
4a+2b=8.
\end{cases}
$$
 
Apply $R_2\leftarrow R_2-4R_1$: $-2b=0$, so $b=0$. Then $a=2$.
 
**Check.**
 
$$
\begin{aligned}
p(0) &= 1, \\
p(1) &= 2+1=3, \\
p(2) &= 8+1=9.
\end{aligned}
$$
 
**Answer.** $p(x)=2x^2+1$.
