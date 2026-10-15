Given:

[
A=\begin{pmatrix}
1&2&3\
4&5&6
\end{pmatrix},
\qquad
B=\begin{pmatrix}
1&0\
2&1\
-1&3
\end{pmatrix}.
]

1. Calculate (A^T)

The transpose exchanges rows and columns.

[
\boxed{
A^T=\begin{pmatrix}
1&4\
2&5\
3&6
\end{pmatrix}
}
]

2. Calculate (B^T)

[
\boxed{
B^T=\begin{pmatrix}
1&2&-1\
0&1&3
\end{pmatrix}
}
]

3. Calculate (AB)

Multiply each row of (A) by each column of (B):

[
AB=
\begin{pmatrix}
1\cdot1+2\cdot2+3\cdot(-1)
&
1\cdot0+2\cdot1+3\cdot3
\
4\cdot1+5\cdot2+6\cdot(-1)
&
4\cdot0+5\cdot1+6\cdot3
\end{pmatrix}.
]

Simplifying:

[
\boxed{
AB=\begin{pmatrix}
2&11\
8&23
\end{pmatrix}
}
]

4. Verify the transpose property

The property to verify is:

[
(AB)^T=B^TA^T.
]

First, transpose the product:

[
(AB)^T=
\begin{pmatrix}
2&8\
11&23
\end{pmatrix}.
]

Now calculate (B^TA^T):

[
B^TA^T=
\begin{pmatrix}
1&2&-1\
0&1&3
\end{pmatrix}
\begin{pmatrix}
1&4\
2&5\
3&6
\end{pmatrix}.
]

Multiplying:

[
B^TA^T=
\begin{pmatrix}
1+4-3&4+10-6\
0+2+9&0+5+18
\end{pmatrix}.
]

Therefore,

[
B^TA^T=
\begin{pmatrix}
2&8\
11&23
\end{pmatrix}.
]

Both sides are equal:

[
\boxed{(AB)^T=B^TA^T}
]

The transpose of a product reverses the order of the factors.
