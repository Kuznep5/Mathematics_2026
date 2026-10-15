Exercise 7. Identity Matrix, Zero Matrix, and Powers

Given:

[
A=\begin{pmatrix}
2&1\
0&2
\end{pmatrix}.
]

For a (2\times2) matrix, define the identity matrix and zero matrix as:

[
I=\begin{pmatrix}
1&0\
0&1
\end{pmatrix},
\qquad
0=\begin{pmatrix}
0&0\
0&0
\end{pmatrix}.
]

1. Calculate (AI)

[
AI=
\begin{pmatrix}
2&1\
0&2
\end{pmatrix}
\begin{pmatrix}
1&0\
0&1
\end{pmatrix}.
]

Therefore,

[
\boxed{
AI=\begin{pmatrix}
2&1\
0&2
\end{pmatrix}=A
}
]

2. Calculate (IA)

[
IA=
\begin{pmatrix}
1&0\
0&1
\end{pmatrix}
\begin{pmatrix}
2&1\
0&2
\end{pmatrix}.
]

Therefore,

[
\boxed{IA=A}
]

3. Calculate (A+0)

[
A+0=
\begin{pmatrix}
2+0&1+0\
0+0&2+0
\end{pmatrix}.
]

Therefore,

[
\boxed{A+0=A}
]

4. Calculate (A^2)

By definition, (A^2=AA).

[
A^2=
\begin{pmatrix}
2&1\
0&2
\end{pmatrix}
\begin{pmatrix}
2&1\
0&2
\end{pmatrix}.
]

[
\boxed{
A^2=\begin{pmatrix}
4&4\
0&4
\end{pmatrix}
}
]

5. Calculate (A^3)

By definition, (A^3=A^2A).

[
A^3=
\begin{pmatrix}
4&4\
0&4
\end{pmatrix}
\begin{pmatrix}
2&1\
0&2
\end{pmatrix}.
]

[
\boxed{
A^3=\begin{pmatrix}
8&12\
0&8
\end{pmatrix}
}
]

Explanation and pattern

The identity matrix does not change a matrix when multiplied by it:

[
AI=IA=A.
]

The zero matrix does not change a matrix when added to it:

[
A+0=A.
]

The successive powers are:

[
A=\begin{pmatrix}2&1\0&2\end{pmatrix},
\quad
A^2=\begin{pmatrix}4&4\0&4\end{pmatrix},
\quad
A^3=\begin{pmatrix}8&12\0&8\end{pmatrix}.
]

The diagonal entries double at each multiplication by (A). The upper-right entry follows the pattern (1,4,12,\ldots).

More generally, for every positive integer (n):

[
\boxed{
A^n=
\begin{pmatrix}
2^n&n2^{n-1}\
0&2^n
\end{pmatrix}
}
]
