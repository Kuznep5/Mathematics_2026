### Exercise 9. Composing Transformations
 
Given
 
$$
S=
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix},\qquad R=
\begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix},\qquad x=
\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}.
$$
 
**Computing $RSx$.** The matrix nearest to $x$ acts first, so $S$ acts first.
 
$$
Sx=
\begin{pmatrix}
2 \\
2 \\
\end{pmatrix},\qquad R(Sx)=
\begin{pmatrix}
0\cdot2+(-1)\cdot2 \\
1\cdot2+0\cdot2 \\
\end{pmatrix}=
\begin{pmatrix}
-2 \\
2 \\
\end{pmatrix}
$$
 
**Computing $SRx$.** Now $R$ acts first.
 
$$
Rx=
\begin{pmatrix}
-2 \\
1 \\
\end{pmatrix},\qquad S(Rx)=
\begin{pmatrix}
2\cdot(-2) \\
1\cdot1 \\
\end{pmatrix}=
\begin{pmatrix}
-4 \\
1 \\
\end{pmatrix}
$$
 
**Comparison.** $RSx=(-2,2)^T$ and $SRx=(-4,1)^T$, so the results differ.
 
**Geometric explanation.** In $RSx$ the vector is first stretched along the $x$-axis and then rotated. In $SRx$ the vector is first rotated and then stretched along the $x$-axis. After a rotation by $90^\circ$ the horizontal direction is a different direction of the vector, so the stretching acts on different components.
 
**Verification via the product matrices.**
 
$$
RS=
\begin{pmatrix}
0 & -1 \\
2 & 0 \\
\end{pmatrix},\qquad SR=
\begin{pmatrix}
0 & -2 \\
1 & 0 \\
\end{pmatrix}
$$
 
Then $RSx=(0\cdot1-1\cdot2,\ 2\cdot1+0\cdot2)=(-2,2)$ and $SRx=(0\cdot1-2\cdot2,\ 1\cdot1+0\cdot2)=(-4,1)$, which agrees with the step-by-step computation.
