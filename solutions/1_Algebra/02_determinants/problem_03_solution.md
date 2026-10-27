### Exercise 3. Swapping Two Rows
 
$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 3 & 1 \\
2 & 1 & 1 \\
\end{pmatrix}
$$
 
By Sarrus' rule,
 
$$
\begin{aligned}
\det A &= (1\cdot 3\cdot 1+2\cdot 1\cdot 2+0\cdot 0\cdot 1)-(0\cdot 3\cdot 2+1\cdot 1\cdot 1+2\cdot 0\cdot 1) \\
       &= (3+4+0)-(0+1+0) \\
       &= 6.
\end{aligned}
$$
 
Let $B$ be obtained from $A$ by swapping the first and second rows:
 
$$
B=
\begin{pmatrix}
0 & 3 & 1 \\
1 & 2 & 0 \\
2 & 1 & 1 \\
\end{pmatrix}.
$$
 
**Prediction.** Swapping two rows changes the sign of the determinant, so $\det B=-\det A=-6$.
 
**Verification.**
 
$$
\begin{aligned}
\det B &= (0\cdot 2\cdot 1+3\cdot 0\cdot 2+1\cdot 1\cdot 1)-(1\cdot 2\cdot 2+0\cdot 0\cdot 1+3\cdot 1\cdot 1) \\
       &= (0+0+1)-(4+0+3) \\
       &= -6.
\end{aligned}
$$
 
The calculation confirms the prediction.
