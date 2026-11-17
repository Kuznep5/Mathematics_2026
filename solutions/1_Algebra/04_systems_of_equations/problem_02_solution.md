# Exercise 2. Gaussian Elimination — One Solution

## Question

Solve the system using Gaussian elimination:

$$
\begin{cases}
x+y+z=6, \\
2x-y+z=3, \\
x+2y-z=2.
\end{cases}
$$

After finding the solution, substitute its values into all three original equations and check that each equation holds.

## Solution

**Method.** Form the augmented matrix, eliminate the entries below each pivot, and then use back substitution. The final values must be checked in the original system.

**Step 1. Write the augmented matrix.** The first three columns contain the coefficients of $x$, $y$, and $z$; the last column contains the right-hand sides:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
2 & -1 & 1 & \mid & 3 \\
1 & 2 & -1 & \mid & 2 \\
\end{pmatrix}.
$$

**Step 2. Eliminate $x$ from the second and third rows.** Use the first row as the pivot row:

$$
R_2\leftarrow R_2-2R_1,\qquad R_3\leftarrow R_3-R_1.
$$

This gives

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & -3 & -1 & \mid & -9 \\
0 & 1 & -2 & \mid & -4 \\
\end{pmatrix}.
$$

**Step 3. Obtain a pivot in the $y$ column.** Interchange the second and third rows so that the coefficient of $y$ in the second row is $1$:

$$
R_2\leftrightarrow R_3.
$$

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & 1 & -2 & \mid & -4 \\
0 & -3 & -1 & \mid & -9 \\
\end{pmatrix}.
$$

Now eliminate $y$ from the third row by using $R_3\leftarrow R_3+3R_2$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & 1 & -2 & \mid & -4 \\
0 & 0 & -7 & \mid & -21 \\
\end{pmatrix}.
$$

**Step 4. Back substitution.** The last equation gives $-7z=-21$, hence $z=3$. The second equation gives $y-2z=-4$, hence $y=2$. The first equation gives $x+y+z=6$, hence $x=1$:

$$
\begin{aligned}
z &= \frac{-21}{-7}=3, \\
y &= -4+2\cdot3=2, \\
x &= 6-2-3=1.
\end{aligned}
$$

**Step 5. Check all three original equations.** Substitute $(x,y,z)=(1,2,3)$:

$$
\begin{aligned}
x+y+z &= 1+2+3=6, \\
2x-y+z &= 2\cdot1-2+3=3, \\
x+2y-z &= 1+2\cdot2-3=2.
\end{aligned}
$$

All three equalities hold, so the solution is consistent with the original equations. Since there is a pivot in each of the three variable columns, the solution is unique.

### Answer

$$
(x,y,z)=(1,2,3).
$$
