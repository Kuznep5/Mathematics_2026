# Exercise 5. A 3×3 Matrix
 
## Question
 
Use Gauss–Jordan elimination to find the inverse of
 
$$
A=
\begin{pmatrix}
1 & 1 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1 \\
\end{pmatrix}.
$$
 
Check the result by multiplication.
 
## Solution
 
**Method.** The $2\times2$ formula does not apply to a $3\times3$ matrix, so we use Gauss–Jordan elimination on $[A\mid I]$. First we create zeros below the diagonal (forward pass), then normalize the pivots and create zeros above the diagonal (backward pass). Every operation is applied to the whole row, including the right block.
 
**Invertibility check.** Expanding the determinant along the first row:
 
$$
\det A = 1\cdot(1\cdot1-1\cdot0)-1\cdot(0\cdot1-1\cdot1)+0 = 1+1 = 2\neq0.
$$
 
The determinant is nonzero, so the elimination will end with $I$ on the left.
 
**Step 0. The augmented matrix.**
 
$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
1 & 0 & 1 & \mid & 0 & 0 & 1 \\
\end{pmatrix}
$$
 
**Step 1.** Clear the first entry of the third row: $R_3\to R_3-R_1$.
 
$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
0 & -1 & 1 & \mid & -1 & 0 & 1 \\
\end{pmatrix}
$$
 
**Step 2.** Clear the second entry of the third row using the second row: $R_3\to R_3+R_2$.
 
$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
0 & 0 & 2 & \mid & -1 & 1 & 1 \\
\end{pmatrix}
$$
 
**Step 3.** Make the third pivot equal to $1$: $R_3\to\frac{1}{2}R_3$.
 
$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
0 & 0 & 1 & \mid & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2} \\
\end{pmatrix}
$$
 
**Step 4.** Clear the entry above the third pivot: $R_2\to R_2-R_3$.
 
$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 0 & \mid & \frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
0 & 0 & 1 & \mid & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2} \\
\end{pmatrix}
$$
 
**Step 5.** Clear the entry above the second pivot: $R_1\to R_1-R_2$.
 
$$
\begin{pmatrix}
1 & 0 & 0 & \mid & \frac{1}{2} & -\frac{1}{2} & \frac{1}{2} \\
0 & 1 & 0 & \mid & \frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
0 & 0 & 1 & \mid & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2} \\
\end{pmatrix}
$$
 
The left block is $I$, so the right block is $A^{-1}$. Factoring out $\frac12$:
 
$$
A^{-1}=
\frac{1}{2}
\begin{pmatrix}
1 & -1 & 1 \\
1 & 1 & -1 \\
-1 & 1 & 1 \\
\end{pmatrix}.
$$
 
**Check by multiplication.** The product $AA^{-1}$ must equal $I$:
 
$$
AA^{-1}=
\frac{1}{2}
\begin{pmatrix}
1 & 1 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & -1 & 1 \\
1 & 1 & -1 \\
-1 & 1 & 1 \\
\end{pmatrix}
$$
 
For example, the entry $(1,1)$ is $1\cdot1+1\cdot1+0\cdot(-1)=2$ and the entry $(1,2)$ is $1\cdot(-1)+1\cdot1+0\cdot1=0$. Computing all entries in the same way:
 
$$
AA^{-1}=
\frac{1}{2}
\begin{pmatrix}
2 & 0 & 0 \\
0 & 2 & 0 \\
0 & 0 & 2 \\
\end{pmatrix}
=I.
$$
