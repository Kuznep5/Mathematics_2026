## Exercise 4. Matrix Multiplication and Noncommutativity

Given:

$$
A=\begin{pmatrix}
1&2\\
0&1
\end{pmatrix},
\qquad
B=\begin{pmatrix}
2&0\\
3&1
\end{pmatrix}.
$$

### 1. Calculate \(AB\)

To multiply two matrices, multiply each row of the first matrix by each column of the second matrix.

$$
AB=
\begin{pmatrix}
1\cdot2+2\cdot3 & 1\cdot0+2\cdot1\\
0\cdot2+1\cdot3 & 0\cdot0+1\cdot1
\end{pmatrix}.
$$

Simplifying:

$$
AB=
\begin{pmatrix}
2+6&0+2\\
0+3&0+1
\end{pmatrix}.
$$

Therefore:

$$
\boxed{
AB=\begin{pmatrix}
8&2\\
3&1
\end{pmatrix}
}
$$

### 2. Calculate \(BA\)

Now reverse the order of the matrices.

$$
BA=
\begin{pmatrix}
2\cdot1+0\cdot0 & 2\cdot2+0\cdot1\\
3\cdot1+1\cdot0 & 3\cdot2+1\cdot1
\end{pmatrix}.
$$

Simplifying:

$$
BA=
\begin{pmatrix}
2+0&4+0\\
3+0&6+1
\end{pmatrix}.
$$

Therefore:

$$
\boxed{
BA=\begin{pmatrix}
2&4\\
3&7
\end{pmatrix}
}
$$

### 3. Compare the results

We obtained:

$$
AB=\begin{pmatrix}
8&2\\
3&1
\end{pmatrix}
$$

and

$$
BA=\begin{pmatrix}
2&4\\
3&7
\end{pmatrix}.
$$

The matrices are different:

$$
\boxed{AB\neq BA}
$$

### Conclusion

Matrix multiplication is not commutative in general. This means that changing the order of the matrices can change the result.

In this example, \(AB\) and \(BA\) are different, so the order of multiplication matters.
