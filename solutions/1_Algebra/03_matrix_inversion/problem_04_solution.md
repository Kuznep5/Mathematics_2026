# Exercise 4. Gauss–Jordan
 
## Question
 
Find $A^{-1}$ using the Gauss–Jordan method for
 
$$
A=
\begin{pmatrix}
1 & 2 \\
3 & 5 \\
\end{pmatrix}.
$$
 
Show the augmented matrix $[A\mid I]$ after successive operations and explain why obtaining $I$ on the left gives the inverse on the right.
 
## Solution
 
**Method.** In the Gauss–Jordan method we write the augmented matrix $[A\mid I]$ and apply elementary row operations to the whole rows, both left and right of the bar, until the left block becomes $I$. The right block then becomes $A^{-1}$. We work column by column: first make the diagonal entry equal to $1$, then clear the other entries of the same column.
 
**Step 0. The augmented matrix.**
 
$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
3 & 5 & \mid & 0 & 1 \\
\end{pmatrix}
$$
 
**Step 1. Clear the entry below the first pivot.** The pivot $1$ in position $(1,1)$ is already correct. To turn the $3$ below it into $0$, subtract $3$ times the first row from the second row: $R_2\to R_2-3R_1$. For the second row this gives $3-3\cdot1=0$, $5-3\cdot2=-1$, $0-3\cdot1=-3$, $1-3\cdot0=1$.
 
$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & -1 & \mid & -3 & 1 \\
\end{pmatrix}
$$
 
**Step 2. Make the second pivot equal to $1$.** The entry in position $(2,2)$ is $-1$, so multiply the second row by $-1$: $R_2\to -R_2$.
 
$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}
$$
 
**Step 3. Clear the entry above the second pivot.** Subtract $2$ times the second row from the first row: $R_1\to R_1-2R_2$. This gives $2-2\cdot1=0$, $1-2\cdot3=-5$, $0-2\cdot(-1)=2$.
 
$$
\begin{pmatrix}
1 & 0 & \mid & -5 & 2 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}
$$
 
The left block is $I$, so the right block is the inverse:
 
$$
A^{-1}=
\begin{pmatrix}
-5 & 2 \\
3 & -1 \\
\end{pmatrix}.
$$
 
**Why obtaining $I$ on the left gives the inverse on the right.** Each elementary row operation is the same as multiplying on the left by an invertible elementary matrix $E_k$. Here the three operations correspond to
 
$$
E_1=
\begin{pmatrix}
1 & 0 \\
-3 & 1 \\
\end{pmatrix},\qquad
E_2=
\begin{pmatrix}
1 & 0 \\
0 & -1 \\
\end{pmatrix},\qquad
E_3=
\begin{pmatrix}
1 & -2 \\
0 & 1 \\
\end{pmatrix}.
$$
 
Reducing the left block to $I$ means
 
$$
E_3E_2E_1A=I,
$$
 
so by the definition of the inverse, $E_3E_2E_1=A^{-1}$. The same operations are applied to the right block, which starts as $I$, hence at the end it equals $E_3E_2E_1I=E_3E_2E_1=A^{-1}$.
 
**Check.** The determinant is $\det A=1\cdot5-2\cdot3=-1$, so the $2\times2$ formula gives
 
$$
A^{-1}=
\frac{1}{-1}
\begin{pmatrix}
5 & -2 \\
-3 & 1 \\
\end{pmatrix}
$$
 
which is the same matrix as above. Multiplying also confirms it:
 
$$
AA^{-1}=
\begin{pmatrix}
1 & 2 \\
3 & 5 \\
\end{pmatrix}
\begin{pmatrix}
-5 & 2 \\
3 & -1 \\
\end{pmatrix}
$$
 
Hence
 
$$
AA^{-1}=
\begin{pmatrix}
-5+6 & 2-2 \\
-15+15 & 6-5 \\
\end{pmatrix}
=I.
$$
