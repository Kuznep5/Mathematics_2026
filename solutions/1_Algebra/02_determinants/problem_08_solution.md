# Exercise 8. Determinant of a Product

## Question

Let $A,B$ be square matrices such that $\det A=3$ and $\det B=-5$. Compute $\det(AB)$, $\det(BA)$ and, if it exists, $\det(A^{-1}B)$. Explain why the first two results are equal even though usually $AB\neq BA$.

## Solution

### Given

$A$ and $B$ are square matrices of the same size, $\det A=3$ and $\det B=-5$.

### Find

The values $\det(AB)$, $\det(BA)$, $\det(A^{-1}B)$ if it exists, and an explanation of why $\det(AB)=\det(BA)$.

### Method and steps

*Step 1. Use multiplicativity.* For square matrices of the same size, $\det(XY)=\det X\cdot\det Y$.

Step 2. Compute $\det(AB)$.

$$
\det(AB) = \det A\cdot\det B = 3\cdot(-5) = -15.
$$

*Step 3. Compute $\det(BA)$.*

$$
\det(BA) = \det B\cdot\det A = (-5)\cdot 3 = -15.
$$

*Step 4. Check that $A^{-1}$ exists.* Since $\det A=3\neq0$, the matrix $A$ is invertible, so $A^{-1}B$ is defined.

*Step 5. Find $\det(A^{-1})$.* From $AA^{-1}=I$ and $\det I=1$ we get $\det A\cdot\det(A^{-1})=1$, so

$$
\det(A^{-1}) = \frac{1}{\det A} = \frac{1}{3}.
$$

*Step 6. Compute $\det(A^{-1}B)$.*

$$
\det(A^{-1}B) = \det(A^{-1})\cdot\det B = \frac{1}{3}\cdot(-5) = -\frac{5}{3}.
$$

*Step 7. Explain $\det(AB)=\det(BA)$.* The matrices $AB$ and $BA$ are usually different. However, their determinants are the products of the same two numbers $\det A$ and $\det B$. Multiplication of real numbers is commutative, so the order of the factors does not matter.

### Answer

$\det(AB)=-15$, $\det(BA)=-15$, $\det(A^{-1}B)=-\dfrac{5}{3}$.
