# Exercise 6. Parameter and Invertibility

## Question

For

$$
A(t)=
\begin{pmatrix}
t & 1 \\
2 & t \\
\end{pmatrix}
$$

find all values of $t$ for which the matrix is not invertible. Explain how your answer is related to the determinant being zero.

## Solution

### Given

A $2\times2$ matrix depending on a real parameter $t$.

### Find

All values of $t$ for which $A(t)$ is not invertible.

### Method and steps

*Step 1. Compute the determinant as a function of $t$.*

$$
\det A(t) = t\cdot t-1\cdot 2 = t^2-2.
$$

*Step 2. Use the criterion.* A square matrix is not invertible exactly when its determinant equals zero. Hence we solve

$$
t^2-2=0.
$$

*Step 3. Solve the equation.* This gives $t^2=2$, so

$$
t=\sqrt{2}, \qquad t=-\sqrt{2}.
$$

*Step 4. Check geometrically.* For $t=\sqrt2$, the second row $(2,\sqrt2)$ equals $\sqrt2$ times the first row $(\sqrt2,1)$. For $t=-\sqrt2$, the second row $(2,-\sqrt2)$ equals $-\sqrt2$ times the first row $(-\sqrt2,1)$. In both cases the rows are proportional, so the matrix is singular. For every other value of $t$ we have $t^2-2\neq0$, and the matrix is invertible.

### Answer

$A(t)$ is not invertible exactly for $t=\sqrt2$ and $t=-\sqrt2$, which are the roots of $\det A(t)=t^2-2$.
