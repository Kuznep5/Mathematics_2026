# Exercise 8. Two Systems with the Same Coefficient Matrix

## Question

Solve the two systems using elimination.

**System 1**

$$
\begin{cases}
2x+y=5, \\
x-y=1.
\end{cases}
$$

**System 2**

$$
\begin{cases}
2x+y=1, \\
x-y=4.
\end{cases}
$$

Compare the successive elimination steps. Explain which part of the calculation is the same in both cases and why.

## Solution

**Method.** Both systems have the same coefficient matrix but different right-hand side vectors:

$$
A=\begin{pmatrix}
2 & 1 \\
1 & -1 \\
\end{pmatrix},\qquad
b_1=\begin{pmatrix}
5 \\
1 \\
\end{pmatrix},\qquad
b_2=\begin{pmatrix}
1 \\
4 \\
\end{pmatrix}.
$$

Use the same row operation in both systems and compare the transformed coefficient entries.

### System 1

**Step 1. Write the augmented matrix.**

$$
\begin{pmatrix}
2 & 1 & \mid & 5 \\
1 & -1 & \mid & 1 \\
\end{pmatrix}.
$$

**Step 2. Eliminate $x$ from the second row.** Apply $R_2\leftarrow 2R_2-R_1$:

$$
\begin{pmatrix}
2 & 1 & \mid & 5 \\
0 & -3 & \mid & -3 \\
\end{pmatrix}.
$$

The second row gives $-3y=-3$, so $y=1$. The first row then gives $2x+1=5$, so $x=2$.

**Verification.** $2\cdot2+1=5$ and $2-1=1$.

### System 2

**Step 1. Write the augmented matrix.**

$$
\begin{pmatrix}
2 & 1 & \mid & 1 \\
1 & -1 & \mid & 4 \\
\end{pmatrix}.
$$

**Step 2. Apply the same elimination operation.** Again use $R_2\leftarrow 2R_2-R_1$:

$$
\begin{pmatrix}
2 & 1 & \mid & 1 \\
0 & -3 & \mid & 7 \\
\end{pmatrix}.
$$

The second row gives $-3y=7$, hence $y=-\frac73$. Substitution into the first row gives

$$
2x=1-y=1+\frac73=\frac{10}{3},\qquad x=\frac53.
$$

**Verification.**

$$
\begin{aligned}
2\cdot\frac53-\frac73 &= \frac{10}{3}-\frac73=1, \\
\frac53-\left(-\frac73\right) &= \frac{12}{3}=4.
\end{aligned}
$$

### Comparison of the elimination steps

In both systems the operation is $R_2\leftarrow2R_2-R_1$. The coefficient rows change in exactly the same way:

$$
\begin{pmatrix}
2 & 1 \\
1 & -1 \\
\end{pmatrix}
\quad\longrightarrow\quad
\begin{pmatrix}
2 & 1 \\
0 & -3 \\
\end{pmatrix}.
$$

Only the right-hand sides change: the lower entry becomes $2\cdot1-5=-3$ in System 1, but $2\cdot4-1=7$ in System 2. The elimination step is shared because the coefficient matrix $A$ is identical in both systems. Different right-hand sides lead to different solutions after the same coefficient reduction.

### Answer

System 1: $(x,y)=(2,1)$. System 2: $(x,y)=(\frac53,-\frac73)$. The elimination of the coefficient matrix is the reusable part.
