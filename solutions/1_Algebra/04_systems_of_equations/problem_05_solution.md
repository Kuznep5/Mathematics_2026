### Exercise 5. Row Echelon Form and Number of Solutions
 
**Problem.** For the augmented matrix
 
$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 3 \\
0 & 1 & 2 & \mid & 1 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$
 
determine the number of solutions and write them in parametric form.
 
**Solution.** The last row is $0=0$ and gives no condition. There are 2 nonzero rows (2 pivots) and 3 unknowns, so $3-2=1$ variable is free. The third column has no pivot, so $z=t$.
 
From row 2: $y+2z=1$, so $y=1-2t$.
 
From row 1: $x+2y-z=3$, so
 
$$
x=3-2(1-2t)+t=1+5t.
$$
 
**Check for $t=0$.** The point is $(1,1,0)$: $1+2-0=3$ and $1+0=1$.
 
**Answer.** Infinitely many solutions: $(x,y,z)=(1+5t,\;1-2t,\;t)$, $t\in\mathbb{R}$. The number of free variables equals the number of unknowns minus the number of pivots.
