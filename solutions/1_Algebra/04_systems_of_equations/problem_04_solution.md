# Exercise 4. Infinitely Many Solutions

## Question

Solve the system

$$
\begin{cases}
x+y+z=2, \\
2x+2y+2z=4, \\
x-y+z=0.
\end{cases}
$$

Give all solutions in parametric form. Identify a free variable and choose one parameter value to verify that the corresponding point satisfies all three original equations.

## Solution

**Method.** Use Gaussian elimination to identify the independent equations and the free variable. Express the other unknowns in terms of a parameter.

**Step 1. Write the augmented matrix.**

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
2 & 2 & 2 & \mid & 4 \\
1 & -1 & 1 & \mid & 0 \\
\end{pmatrix}.
$$

**Step 2. Eliminate $x$ from rows 2 and 3.** Apply

$$
R_2\leftarrow R_2-2R_1,\qquad R_3\leftarrow R_3-R_1.
$$

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & 0 & 0 & \mid & 0 \\
0 & -2 & 0 & \mid & -2 \\
\end{pmatrix}.
$$

The second row is $0=0$, so it supplies no additional restriction. Move the third row into the second position and divide it by $-2$:

$$
R_2\leftrightarrow R_3,\qquad R_2\leftarrow -\frac12R_2.
$$

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & 1 & 0 & \mid & 1 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}.
$$

**Step 3. Choose the free variable.** The pivots are in the $x$ and $y$ columns, but not in the $z$ column. Therefore $z$ is free. Write $z=t$, where $t\in\mathbb{R}$.

The second row gives $y=1$, and the first row then gives

$$
x=2-y-z=2-1-t=1-t.
$$

Thus every solution has the form

$$
(x,y,z)=(1-t,1,t),\qquad t\in\mathbb{R}.
$$

**Step 4. Check one parameter value.** Choose $t=2$. Then $(x,y,z)=(-1,1,2)$. Substitution into the original equations gives

$$
\begin{aligned}
x+y+z &= -1+1+2=2, \\
2x+2y+2z &= 2(-1)+2(1)+2(2)=4, \\
x-y+z &= -1-1+2=0.
\end{aligned}
$$

All three equations hold. As $t$ can be any real number, there are infinitely many solutions.

### Answer

$$
(x,y,z)=(1-t,1,t),\qquad t\in\mathbb{R}.
$$
