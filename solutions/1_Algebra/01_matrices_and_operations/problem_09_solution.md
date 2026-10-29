# Exercise 9. Composing Transformations

## Question

Let

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix},\qquad R=
\begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix}.
$$

The matrix $S$ describes nonuniform scaling, while $R$ describes a $90^\circ$ counterclockwise rotation.
For

$$
x=
\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}
$$

compute $RSx$ and $SRx$. Compare the results and explain geometrically why the order of these transformations matters.

## Solution

In a product such as $RSx$ the matrix nearest to the vector acts first. Thus in $RSx$ the scaling $S$ acts first and then the rotation $R$, while in $SRx$ the rotation acts first and then the scaling.

**Computing $RSx$.** First the scaling:

$$
Sx=
\begin{pmatrix}
2\cdot1+0\cdot2 \\
0\cdot1+1\cdot2 \\
\end{pmatrix}=
\begin{pmatrix}
2 \\
2 \\
\end{pmatrix}.
$$

Then the rotation is applied to this result:

$$
R(Sx)=
\begin{pmatrix}
0\cdot2+(-1)\cdot2 \\
1\cdot2+0\cdot2 \\
\end{pmatrix}=
\begin{pmatrix}
-2 \\
2 \\
\end{pmatrix}.
$$

**Computing $SRx$.** First the rotation:

$$
Rx=
\begin{pmatrix}
0\cdot1+(-1)\cdot2 \\
1\cdot1+0\cdot2 \\
\end{pmatrix}=
\begin{pmatrix}
-2 \\
1 \\
\end{pmatrix}.
$$

Then the scaling is applied to this result:

$$
S(Rx)=
\begin{pmatrix}
2\cdot(-2)+0\cdot1 \\
0\cdot(-2)+1\cdot1 \\
\end{pmatrix}=
\begin{pmatrix}
-4 \\
1 \\
\end{pmatrix}.
$$

**Comparison.** $RSx=(-2,2)^T$ and $SRx=(-4,1)^T$, so the results differ.

**Geometric explanation.** In $RSx$ the vector is first stretched along the $x$-axis and then rotated. In $SRx$ the vector is first rotated and then stretched along the $x$-axis. After a rotation by $90^\circ$ the horizontal and vertical components of the vector have exchanged roles, so the stretching along the $x$-axis acts on different components. This is why the order of the transformations matters.

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
\end{pmatrix}.
$$

Then $RSx=(0\cdot1-1\cdot2,\ 2\cdot1+0\cdot2)^T=(-2,2)^T$ and $SRx=(0\cdot1-2\cdot2,\ 1\cdot1+0\cdot2)^T=(-4,1)^T$, which agrees with the step-by-step computation. Also $RS\neq SR$.
