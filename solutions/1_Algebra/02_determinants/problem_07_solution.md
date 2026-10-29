# Exercise 7. Using Properties Instead of Recomputing

## Question

Suppose that for a $3\times3$ matrix, $\det A=-4$. Compute

$$
\det(2A),\qquad \det(A^T),\qquad \det(A^2),\qquad \det(-A).
$$

Justify each answer using the appropriate property.

## Solution

### Given

$A$ is a $3\times3$ matrix and $\det A=-4$.

### Find

The values $\det(2A)$, $\det(A^T)$, $\det(A^2)$ and $\det(-A)$, with justification.

### Method and steps

*Step 1. Compute $\det(2A)$.* Multiplying the whole matrix by $2$ multiplies each of its $3$ rows by $2$. Each row multiplied by a number multiplies the determinant by that number, so the determinant is multiplied by $2^3$:

$$
\det(2A) = 2^3\det A = 8\cdot(-4) = -32.
$$

*Step 2. Compute $\det(A^T)$.* A matrix and its transpose have the same determinant:

$$
\det(A^T) = \det A = -4.
$$

*Step 3. Compute $\det(A^2)$.* The determinant is multiplicative, that is, $\det(XY)=\det X\cdot\det Y$. Taking $X=Y=A$ gives

$$
\det(A^2) = (\det A)^2 = (-4)^2 = 16.
$$

*Step 4. Compute $\det(-A)$.* This is the case $c=-1$ of Step 1, so the determinant is multiplied by $(-1)^3=-1$:

$$
\det(-A) = (-1)^3\det A = -(-4) = 4.
$$

### Answer

$\det(2A)=-32$, $\det(A^T)=-4$, $\det(A^2)=16$, $\det(-A)=4$.
