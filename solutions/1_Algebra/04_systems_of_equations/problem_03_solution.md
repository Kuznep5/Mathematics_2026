# Exercise 3. Inconsistent System

## Question

Solve the system or show that it is inconsistent:

$$
\begin{cases}
x+2y=3, \\
2x+4y=7.
\end{cases}
$$

Show how a contradiction appears in the augmented matrix after elimination, and explain the contradiction in terms of the original equations.

## Solution

**Method.** Perform a row operation on the augmented matrix. If a row becomes a zero expression on the left equal to a nonzero constant on the right, the equations cannot be satisfied simultaneously.

**Step 1. Write the augmented matrix.**

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
2 & 4 & \mid & 7 \\
\end{pmatrix}.
$$

**Step 2. Eliminate $x$ from the second row.** Subtract twice the first row from the second:

$$
R_2\leftarrow R_2-2R_1.
$$

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
0 & 0 & \mid & 1 \\
\end{pmatrix}.
$$

**Step 3. Interpret the contradiction.** The last row represents

$$
0x+0y=1,\qquad 0=1.
$$

This is impossible, so no ordered pair $(x,y)$ can satisfy the system.

**Step 4. Interpret the original equations.** Twice the first equation would give $2x+4y=6$, while the second equation requires $2x+4y=7$. The same expression cannot equal both $6$ and $7$. Geometrically, the equations describe distinct parallel lines, so they have no intersection point.

### Answer

The system is **inconsistent** and has **no solution**.
