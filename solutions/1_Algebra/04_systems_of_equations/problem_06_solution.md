# Exercise 6. A System with a Parameter — Which Cases Actually Occur?

## Question

Analyze the system depending on the real parameter $a$:

$$
\begin{cases}
x+y=2, \\
ax+ay=4.
\end{cases}
$$

Determine for which values of $a$ each of the three possibilities occurs: exactly one solution, infinitely many solutions, or no solution. If one type of solution cannot occur, explain why.

## Solution

**Method.** Eliminate the variable terms in the second row. The resulting equation will show for which parameter values the system is consistent.

**Step 1. Form the augmented matrix.**

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
a & a & \mid & 4 \\
\end{pmatrix}.
$$

**Step 2. Eliminate the second row's coefficients.** Apply

$$
R_2\leftarrow R_2-aR_1.
$$

The result is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 4-2a \\
\end{pmatrix}.
$$

The last row represents $0=4-2a$, and the outcome depends on whether the right-hand side is zero.

**Step 3. Case $a=2$.** Here $4-2a=0$, so the second row becomes $0=0$. Only $x+y=2$ remains. Choose $y=t$, where $t\in\mathbb{R}$; then $x=2-t$:

$$
(x,y)=(2-t,t),\qquad t\in\mathbb{R}.
$$

There are infinitely many solutions. Indeed, the second original equation is $2x+2y=4$, exactly twice the first.

**Step 4. Case $a\neq2$.** Here $4-2a\neq0$, so the last row is a contradiction:

$$
0=4-2a\neq0.
$$

Therefore the system has no solution for all $a\neq2$.

**Step 5. Explain why a unique solution cannot occur.** The coefficient row $(a,a)$ is always $a$ times $(1,1)$. Thus the coefficient matrix can never have two pivots. When the equations are consistent, they leave one free variable; when they are inconsistent, there is no solution. Exactly one solution is impossible for every $a$.

### Answer

- If $a=2$, there are infinitely many solutions: $(x,y)=(2-t,t)$ for $t\in\mathbb{R}$.
- If $a\neq2$, there is no solution.
- There is no parameter value for which the system has exactly one solution.
