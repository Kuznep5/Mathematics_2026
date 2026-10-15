## Exercise 8 — Determinant of a Matrix

Given:

$$
A =
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3
\end{pmatrix}
$$

Calculate the determinant:

$$
\det(A)=
1\begin{vmatrix}4&1\\1&3\end{vmatrix}
-2\begin{vmatrix}2&1\\-1&3\end{vmatrix}
+(-1)\begin{vmatrix}2&4\\-1&1\end{vmatrix}
$$

For a \(2\times2\) matrix:

$$
\begin{vmatrix}a&b\\c&d\end{vmatrix}=ad-bc
$$

Therefore:

$$
\det(A)=1(4\cdot3-1\cdot1)
-2(2\cdot3-1\cdot(-1))
+(-1)(2\cdot1-4\cdot(-1))
$$

$$
\det(A)=1(11)-2(7)+(-1)(6)
$$

$$
\det(A)=11-14-6=-9
$$

**Final answer:**

$$
\boxed{\det(A)=-9}
$$
