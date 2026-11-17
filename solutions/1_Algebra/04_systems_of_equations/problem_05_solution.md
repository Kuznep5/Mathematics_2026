# Exercise 5. Row Echelon Form and Number of Solutions

## Question

For the augmented matrix

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 3 \\
0 & 1 & 2 & \mid & 1 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

determine the number of solutions and write all solutions in parametric form. Explain how the matrix shows how many variables may be chosen freely.

## Solution

**Method.** The augmented matrix is already in row echelon form. Identify its pivot columns, choose a parameter for each nonpivot variable, and solve by back substitution.

**Step 1. Convert the rows into equations.** The variable columns correspond to $x$, $y$, and $z$:

$$
\begin{cases}
x+2y-z=3, \\
y+2z=1, \\
0=0.
\end{cases}
$$

The last row is always true, so the system is consistent.

**Step 2. Count the free variables.** There are three unknowns, but only two pivot positions, in columns $x$ and $y$. The number of free variables is

$$
3-2=1.
$$

Thus $z$ is the only free variable; let $z=t$, with $t\in\mathbb{R}$.

**Step 3. Back substitution.** From the second equation,

$$
y+2t=1\quad\Rightarrow\quad y=1-2t.
$$

Insert this expression and $z=t$ into the first equation:

$$
\begin{aligned}
x+2(1-2t)-t &= 3, \\
x+2-5t &= 3, \\
x &= 1+5t.
\end{aligned}
$$

**Step 4. Check.** Substituting the general result into the two nonzero equations gives

$$
\begin{aligned}
(1+5t)+2(1-2t)-t &= 3, \\
(1-2t)+2t &= 1.
\end{aligned}
$$

Both identities hold for every real $t$, while the third row is $0=0$. Therefore the system has infinitely many solutions.

### Answer

$$
(x,y,z)=(1+5t,1-2t,t),\qquad t\in\mathbb{R}.
$$

There is one free variable because the three variable columns contain only two pivots.
