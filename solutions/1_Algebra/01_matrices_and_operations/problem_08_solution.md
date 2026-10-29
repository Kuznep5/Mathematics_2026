# Exercise 8. Row Operations and Their Reversibility

## Question

For

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3 \\
\end{pmatrix}
$$

perform, in order:

1. $R_2\leftarrow R_2-2R_1$,
2. $R_3\leftarrow R_3+R_1$,
3. interchange $R_2$ and $R_3$.

Write the matrix after each step. Then, for each of the three operations, state an operation that reverses it.

## Solution

The notation $R_2\leftarrow R_2-2R_1$ means: subtract $2$ times the first row from the second row and write the result in place of the second row. The first row is not changed.

**Step 1.** $R_2\leftarrow R_2-2R_1$. Since $2R_1=(2,4,-2)$, the new second row is $(2-2,\ 4-4,\ 1-(-2))=(0,0,3)$:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3 \\
\end{pmatrix}.
$$

**Step 2.** $R_3\leftarrow R_3+R_1$. The new third row is $(-1+1,\ 1+2,\ 3+(-1))=(0,3,2)$:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2 \\
\end{pmatrix}.
$$

**Step 3.** Interchange $R_2$ and $R_3$. The second and third rows simply change places:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3 \\
\end{pmatrix}.
$$

**Reversing operations.** Each operation can be undone by an operation of the same kind:

| Operation | Reversing operation |
|---|---|
| $R_2\leftarrow R_2-2R_1$ | $R_2\leftarrow R_2+2R_1$ |
| $R_3\leftarrow R_3+R_1$ | $R_3\leftarrow R_3-R_1$ |
| interchange $R_2$ and $R_3$ | interchange $R_2$ and $R_3$ again |

**Verification.** The reversing operations are applied in the opposite order. Undoing the interchange gives back the rows $(0,0,3)$ and $(0,3,2)$ in positions 2 and 3. Then $R_3\leftarrow R_3-R_1$ gives $(0,3,2)-(1,2,-1)=(-1,1,3)$, which is the original third row. Finally $R_2\leftarrow R_2+2R_1$ gives $(0,0,3)+(2,4,-2)=(2,4,1)$, which is the original second row. The original matrix $A$ is recovered, so no information was lost.
