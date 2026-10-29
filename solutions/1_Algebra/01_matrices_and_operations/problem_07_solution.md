# Exercise 7. Identity Matrix, Zero Matrix, and Powers

## Question

For

$$
A=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

compute

$$
AI,\qquad IA,\qquad A+0,\qquad A^2,\qquad A^3.
$$

Explain the roles of the matrices $I$ and $0$, and describe the pattern you observe in successive powers of $A$.

## Solution

**Neutral elements.** Here $I$ is the $2\times2$ identity matrix (ones on the diagonal, zeros elsewhere) and $0$ is the $2\times2$ zero matrix. They satisfy

$$
AI=A,\qquad IA=A,\qquad A+0=A.
$$

For example,

$$
AI=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}.
$$

The matrix $I$ plays the role of the number $1$ in multiplication, and the matrix $0$ plays the role of the number $0$ in addition.

**Powers.** The square is $A^2=AA$:

$$
A^2=
\begin{pmatrix}
2\cdot2+1\cdot0 & 2\cdot1+1\cdot2 \\
0\cdot2+2\cdot0 & 0\cdot1+2\cdot2 \\
\end{pmatrix}=
\begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix}.
$$

The cube is $A^3=A^2A$:

$$
A^3=
\begin{pmatrix}
4\cdot2+4\cdot0 & 4\cdot1+4\cdot2 \\
0\cdot2+4\cdot0 & 0\cdot1+4\cdot2 \\
\end{pmatrix}=
\begin{pmatrix}
8 & 12 \\
0 & 8 \\
\end{pmatrix}.
$$

**Pattern.** The diagonal entries are $2,4,8$, that is $2^n$. The upper right entries are $1,4,12$, that is $n\cdot2^{n-1}$. The lower left entry stays $0$. Hence

$$
A^n=
\begin{pmatrix}
2^n & n\cdot2^{n-1} \\
0 & 2^n \\
\end{pmatrix}.
$$

**Verification.** For $n=2$ the formula gives $2^2=4$ and $2\cdot2=4$. For $n=3$ it gives $2^3=8$ and $3\cdot4=12$. Both agree with the direct computation.
