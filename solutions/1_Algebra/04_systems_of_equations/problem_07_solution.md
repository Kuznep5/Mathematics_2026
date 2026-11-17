# Exercise 7. Choosing a Method Deliberately

## Question

Do not solve all the following systems completely. For each situation, choose the method that best uses its structure and justify the choice.

**Case 1.** A system with a triangular coefficient matrix:

$$
\begin{cases}
2x-y=3, \\
4y=8.
\end{cases}
$$

**Case 2.** Three systems $Ax=b_i$, for $i=1,2,3$, with the same invertible coefficient matrix $A$, when $A^{-1}$ is already known.

**Case 3.** One $3\times3$ system for which the inverse matrix is not given, and the goal is to find only one solution vector.

For Case 1, carry out the selected method completely. For Cases 2 and 3, describe the plan and identify which computation could be reused or would be unnecessary. Justify the choices using the structure of the matrix and the number of right-hand sides, rather than the method's name alone.

## Solution

**Method.** A triangular matrix can be solved directly by substitution. When several systems share a coefficient matrix, work already performed on that matrix may be reused. For one system with an unknown inverse, elimination generally avoids computing unnecessary information.

### Case 1. Triangular system

**Step 1. Recognize the structure.** The coefficient matrix is

$$
A=\begin{pmatrix}
2 & -1 \\
0 & 4 \\
\end{pmatrix}.
$$

The entry below the main diagonal is zero, so the matrix is upper triangular. The last equation contains only $y$. Back substitution requires no preliminary elimination.

**Step 2. Solve the last equation.**

$$
4y=8\quad\Rightarrow\quad y=2.
$$

**Step 3. Substitute into the first equation.**

$$
\begin{aligned}
2x-y &= 3, \\
2x-2 &= 3, \\
2x &= 5, \\
x &= \frac52.
\end{aligned}
$$

**Verification.** Substitution gives $2\cdot\frac52-2=3$ and $4\cdot2=8$. Thus the solution is $(x,y)=(\frac52,2)$.

### Case 2. Same invertible matrix and three right-hand sides

**Step 1. Use the known inverse.** For each $i=1,2,3$, multiply the equation $Ax_i=b_i$ on the left by $A^{-1}$:

$$
A^{-1}Ax_i=A^{-1}b_i\quad\Rightarrow\quad x_i=A^{-1}b_i.
$$

**Step 2. Identify reusable work.** The same known matrix $A^{-1}$ is used for all three right-hand sides. Only the matrix-vector products with $b_1$, $b_2$, and $b_3$ need to be computed. Recalculating the inverse or repeating elimination for each $b_i$ would be unnecessary.

Because there are three right-hand sides and the inverse is already available, reusing $A^{-1}$ directly is efficient.

### Case 3. One system of size $3\times3$, no known inverse

**Step 1. Choose elimination.** Form the augmented matrix $[A\mid b]$ and use Gaussian elimination to produce row echelon form.

**Step 2. Finish only the required calculation.** Use back substitution to obtain the solution vector, if the system has a unique solution. If the elimination shows a contradiction or a free variable, report the corresponding solution type instead.

**Step 3. Identify unnecessary work.** Computing all of $A^{-1}$ would require solving for the three columns of the identity matrix, even though the question concerns only one right-hand side $b$. There are no other right-hand sides for which an inverse or a factorization needs to be reused.

### Answer

Case 1: back substitution, giving $(x,y)=(\frac52,2)$. Case 2: reuse the known inverse and compute $x_i=A^{-1}b_i$ for each $i$. Case 3: apply Gaussian elimination to $[A\mid b]$ and back substitution, without calculating $A^{-1}$.
