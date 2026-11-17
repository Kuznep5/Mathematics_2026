# Exercise 1. From a System to a Matrix

## Question

Write the system

$$
\begin{cases}
2x-y+z=4, \\
x+3y-2z=1, \\
3x+y+z=7.
\end{cases}
$$

in the form $Ax=b$. Identify the coefficient matrix, the vector of unknowns, and the right-hand side vector. Explain how each row of the matrix corresponds to one equation.

## Solution

**Method.** In the matrix equation $Ax=b$, each row of $A$ contains the coefficients of $x$, $y$, and $z$ from one equation, written in that order. The vector $x$ contains the unknowns, and $b$ contains the constants on the right-hand sides.

**Step 1. Identify the coefficient matrix.** The coefficients of $(x,y,z)$ are $(2,-1,1)$ in the first equation, $(1,3,-2)$ in the second, and $(3,1,1)$ in the third. Hence

$$
A=\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1 \\
\end{pmatrix}.
$$

**Step 2. Identify the two vectors.** The unknown vector and the right-hand side vector are

$$
x=\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix},\qquad
b=\begin{pmatrix}
4 \\
1 \\
7 \\
\end{pmatrix}.
$$

The matrix $A$ has size $3\times3$, while both vectors have size $3\times1$, so the product $Ax$ is defined and has size $3\times1$.

**Step 3. Explain the correspondence between rows and equations.** Multiplying each row of $A$ by the column vector of unknowns gives

$$
Ax=\begin{pmatrix}
2x-y+z \\
x+3y-2z \\
3x+y+z \\
\end{pmatrix}.
$$

The first row gives $2x-y+z=4$, the second gives $x+3y-2z=1$, and the third gives $3x+y+z=7$. Thus all three original equations appear in the same order.

**Verification.** Expanding the matrix equation $Ax=b$ reproduces the complete original system, including the signs and right-hand sides.

### Answer

$$
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix}
\;=\;
\begin{pmatrix}
4 \\
1 \\
7 \\
\end{pmatrix}.
$$
