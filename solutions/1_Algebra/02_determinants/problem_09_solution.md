# Exercise 9. Area and the Determinant

## Question

The vectors

$$
u=
\begin{pmatrix}
3 \\
1 \\
\end{pmatrix},
\qquad
v=
\begin{pmatrix}
1 \\
4 \\
\end{pmatrix}
$$

span a parallelogram. Compute its area using a determinant. Then reverse the order of the vectors and explain what changes in the determinant and what does not change in the area.

## Solution

### Given

The vectors $u=(3,1)$ and $v=(1,4)$ in the plane.

### Find

The area of the parallelogram spanned by $u$ and $v$, and the effect of reversing the order of the vectors.

### Method and steps

*Step 1. Recall the geometric meaning.* The area of the parallelogram spanned by two vectors in the plane equals the absolute value of the determinant of the matrix whose columns are these vectors.

*Step 2. Form the matrix and compute.*

$$
\det
\begin{pmatrix}
3 & 1 \\
1 & 4 \\
\end{pmatrix}
= 3\cdot 4-1\cdot 1 = 11.
$$

*Step 3. Take the absolute value.* The area is $|11|=11$.

*Step 4. Reverse the order.* Taking $v$ first and $u$ second swaps the columns:

$$
\det
\begin{pmatrix}
1 & 3 \\
4 & 1 \\
\end{pmatrix}
= 1\cdot 1-3\cdot 4 = -11.
$$

*Step 5. Explain what changed.* Swapping two columns changes the sign of the determinant, so the determinant changes from $11$ to $-11$. The sign records the orientation of the ordered pair of vectors: counterclockwise gives a positive sign, clockwise gives a negative sign.

*Step 6. Explain what did not change.* The parallelogram is the same set of points, so its area is still $|-11|=11$.

### Answer

The area is $11$. Reversing the order changes the determinant from $11$ to $-11$, but the area remains $11$.
