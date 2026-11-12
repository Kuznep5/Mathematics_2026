### Exercise 1. From a System to a Matrix
 
**Problem.** Write the system
 
$$
\begin{cases}
2x-y+z=4, \\
x+3y-2z=1, \\
3x+y+z=7
\end{cases}
$$
 
in the form $Ax=b$.
 
**Solution.** The coefficients of the unknowns $x,y,z$ in each equation form one row of $A$. The right-hand sides form $b$.
 
$$
A=
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1 \\
\end{pmatrix},\qquad x=
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix},\qquad b=
\begin{pmatrix}
4 \\
1 \\
7 \\
\end{pmatrix}
$$
 
Row $i$ of $A$ multiplied by the vector $x$ gives the left-hand side of equation $i$:
 
$$
Ax=
\begin{pmatrix}
2x-y+z \\
x+3y-2z \\
3x+y+z \\
\end{pmatrix}
$$
 
Setting $Ax=b$ compares these three entries with $4$, $1$, $7$, which restores the original three equations.
 
**Answer.** The system is $Ax=b$ with $A$, $x$, $b$ as above.
 
---
