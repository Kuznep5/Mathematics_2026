# Exercise 10. A Polynomial Through Three Points

## Question

Find a polynomial

$$
p(x)=ax^2+bx+c
$$

whose graph passes through the points $(0,1)$, $(1,3)$, and $(2,9)$. Reduce the three point conditions to a system of linear equations for $a$, $b$, and $c$, and check the result by substituting all three points into the polynomial.

## Solution

**Method.** A point $(x_0,y_0)$ lies on the graph if $p(x_0)=y_0$. Each of the three points therefore gives one linear equation in the unknown coefficients $a$, $b$, and $c$.

**Step 1. Translate the point conditions.**

For $(0,1)$, the condition $p(0)=1$ gives $c=1$. For $(1,3)$, the condition $p(1)=3$ gives $a+b+c=3$. For $(2,9)$, the condition $p(2)=9$ gives $4a+2b+c=9$.

Thus the required system is

$$
\begin{cases}
c=1, \\
a+b+c=3, \\
4a+2b+c=9.
\end{cases}
$$

**Step 2. Write the augmented matrix.** Using the column order $a$, $b$, $c$:

$$
\begin{pmatrix}
0 & 0 & 1 & \mid & 1 \\
1 & 1 & 1 & \mid & 3 \\
4 & 2 & 1 & \mid & 9 \\
\end{pmatrix}.
$$

**Step 3. Solve for the coefficients.** From the first equation, $c=1$. Substitute this into the other two equations:

$$
\begin{cases}
a+b=2, \\
4a+2b=8.
\end{cases}
$$

Subtract twice the first equation from the second: $2a=4$, so $a=2$. Then $a+b=2$ gives $b=0$. Together with $c=1$, this yields

$$
a=2,\qquad b=0,\qquad c=1.
$$

Therefore

$$
p(x)=2x^2+1.
$$

**Step 4. Check all three points.**

$$
\begin{aligned}
p(0) &= 2\cdot0^2+1=1, \\
p(1) &= 2\cdot1^2+1=3, \\
p(2) &= 2\cdot2^2+1=9.
\end{aligned}
$$

The graph passes through all three given points. The reduced system determines $a$ and $b$ uniquely, while the first equation fixes $c$, so the polynomial is unique.

### Answer

$$
p(x)=2x^2+1.
$$
