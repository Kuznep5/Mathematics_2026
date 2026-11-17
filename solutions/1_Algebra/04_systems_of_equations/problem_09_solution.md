# Exercise 9. A System from a Sum Condition

## Question

Find the numbers $x$ and $y$ satisfying

$$
x+y=10,\qquad 2x+5y=32.
$$

Solve the system and explain geometrically why its solution is unique.

## Solution

**Method.** Treat the two conditions as a system of linear equations. Use elimination to calculate the intersection point, then compare the slopes of the two lines.

**Step 1. Write the augmented matrix.**

$$
\begin{pmatrix}
1 & 1 & \mid & 10 \\
2 & 5 & \mid & 32 \\
\end{pmatrix}.
$$

**Step 2. Eliminate $x$ from the second row.** Apply $R_2\leftarrow R_2-2R_1$:

$$
\begin{pmatrix}
1 & 1 & \mid & 10 \\
0 & 3 & \mid & 12 \\
\end{pmatrix}.
$$

Thus $3y=12$, giving $y=4$. Substituting into $x+y=10$ gives $x=6$.

**Step 3. Verify the values.**

$$
\begin{aligned}
x+y &= 6+4=10, \\
2x+5y &= 2\cdot6+5\cdot4=12+20=32.
\end{aligned}
$$

**Step 4. Explain geometric uniqueness.** Write each equation as $y$ in terms of $x$:

$$
y=10-x,\qquad y=\frac{32}{5}-\frac25x.
$$

The slopes are $-1$ and $-\frac25$, which are different. The lines are not parallel and therefore intersect at exactly one point. That point is $(6,4)$. The elimination matrix also confirms uniqueness because it has a pivot in each variable column.

### Answer

$$
(x,y)=(6,4).
$$
