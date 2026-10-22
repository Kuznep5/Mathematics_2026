### Exercise 7. Identity Matrix, Zero Matrix, and Powers
 
Given
 
$$
A=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}.
$$
 
**Neutral elements.** For the $2\times2$ identity matrix $I$ and the zero matrix $0$:
 
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
 
**Powers.**
 
$$
A^2=
\begin{pmatrix}
2\cdot2+1\cdot0 & 2\cdot1+1\cdot2 \\
0\cdot2+2\cdot0 & 0\cdot1+2\cdot2 \\
\end{pmatrix}=
\begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix}
$$
 
$$
A^3=A^2A=
\begin{pmatrix}
4\cdot2+4\cdot0 & 4\cdot1+4\cdot2 \\
0\cdot2+4\cdot0 & 0\cdot1+4\cdot2 \\
\end{pmatrix}=
\begin{pmatrix}
8 & 12 \\
0 & 8 \\
\end{pmatrix}
$$
 
**Pattern.** The diagonal entries are $2,4,8$, that is $2^n$. The upper right entries are $1,4,12$, that is $n\cdot2^{n-1}$. Hence
 
$$
A^n=
\begin{pmatrix}
2^n & n\cdot2^{n-1} \\
0 & 2^n \\
\end{pmatrix}.
$$
 
**Verification.** For $n=2$ the formula gives $2^2=4$ and $2\cdot2=4$. For $n=3$ it gives $2^3=8$ and $3\cdot4=12$. Both agree with the direct computation.
 
---
