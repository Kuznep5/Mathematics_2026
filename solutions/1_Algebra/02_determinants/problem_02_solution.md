### Exercise 2. Determinant of a 3×3 Matrix
 
$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
2 & 1 & 5 \\
\end{pmatrix}
$$
 
**Sarrus' rule.** The sum of the products along the three "downward" diagonals is
 
$$
1\cdot 3\cdot 5 + 2\cdot 4\cdot 2 + (-1)\cdot 0\cdot 1 = 15+16+0 = 31.
$$
 
The sum of the products along the three "upward" diagonals is
 
$$
(-1)\cdot 3\cdot 2 + 1\cdot 4\cdot 1 + 2\cdot 0\cdot 5 = -6+4+0 = -2.
$$
 
Therefore
 
$$
\det A = 31-(-2) = 33.
$$
 
**Check.** Replacing $R_3$ by $R_3-2R_1$ does not change the determinant, because adding a multiple of one row to another row preserves it. We obtain
 
$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & -3 & 7 \\
\end{pmatrix}.
$$
 
Expanding along the first column gives
 
$$
\det A = 1\cdot\bigl(3\cdot 7-4\cdot(-3)\bigr) = 21+12 = 33.
$$
 
Both results agree.
