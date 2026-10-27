### Exercise 7. Using Properties Instead of Recomputing
 
Let $A$ be a $3\times 3$ matrix with $\det A=-4$.
 
$$
\begin{aligned}
\det(2A) &= 2^3\det A = 8\cdot(-4) = -32, \\
\det(A^T) &= \det A = -4, \\
\det(A^2) &= (\det A)^2 = 16, \\
\det(-A) &= (-1)^3\det A = -(-4) = 4.
\end{aligned}
$$
 
**Justification.**
 
- Multiplying a $3\times3$ matrix by a scalar $c$ multiplies each of the three rows by $c$, so the determinant is multiplied by $c^3$. This gives the first and fourth results.
- A matrix and its transpose have the same determinant.
- The determinant is multiplicative: $\det(AB)=\det A\det B$, so $\det(A^2)=(\det A)^2$.
