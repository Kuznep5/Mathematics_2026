### Exercise 7. Choosing a Method Deliberately
 
**Case 1.** The system
 
$$
\begin{cases}
2x-y=3, \\
4y=8
\end{cases}
$$
 
is triangular. The best method is back substitution, because no elimination is needed.
 
$$
\begin{aligned}
4y &= 8 \quad\Rightarrow\quad y=2, \\
2x-2 &= 3 \quad\Rightarrow\quad x=\tfrac52.
\end{aligned}
$$
 
Check: $2\cdot\tfrac52-2=3$ and $4\cdot2=8$.
 
**Answer for case 1.** $(x,y)=\left(\tfrac52,\,2\right)$.
 
**Case 2.** Three systems $Ax=b_i$ with the same invertible $A$ and a known $A^{-1}$.
 
Plan: compute $x_i=A^{-1}b_i$ for $i=1,2,3$. Each solution is one matrix-vector multiplication.
 
- Reusable: the matrix $A^{-1}$ is used for all three right-hand sides.
- Unnecessary: repeating elimination on $A$ for every $b_i$.
The method is chosen because there are several right-hand sides and the inverse is already available.
 
**Case 3.** One $3\times3$ system, no inverse given, one solution vector wanted.
 
Plan: Gaussian elimination on the augmented matrix $[A\mid b]$ followed by back substitution.
 
- Unnecessary: computing $A^{-1}$. Finding the inverse requires working with three right-hand sides (the columns of $I$), which is much more work than needed for a single $b$.
- Reusable: nothing needs to be saved, since there is only one right-hand side.
---
