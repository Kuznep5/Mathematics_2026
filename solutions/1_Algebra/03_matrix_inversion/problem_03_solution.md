# Exercise 3. When Does the Inverse Not Exist?
 
## Question
 
For
 
$$
A=
\begin{pmatrix}
2 & 4 \\
1 & 2 \\
\end{pmatrix}
$$
 
explain in two ways why $A^{-1}$ does not exist: using the determinant and using dependence between the rows.
 
## Solution
 
A square matrix is invertible if and only if its determinant is nonzero, which is equivalent to its rows being linearly independent. We show that both conditions fail for the given matrix.
 
**Way 1. The determinant.**
 
$$
\det A = 2\cdot2-4\cdot1 = 4-4 = 0.
$$
 
Since $\det A=0$, the matrix is not invertible. This also agrees with the $2\times2$ inverse formula, which requires dividing by $ad-bc$, and here that number is zero.
 
**Way 2. Dependence between the rows.** The first row is a multiple of the second row:
 
$$
(2,\ 4) = 2\cdot(1,\ 2).
$$
 
So the rows are linearly dependent and the rank of $A$ is $1<2$. A $2\times2$ matrix of rank less than $2$ is not invertible. Geometrically, $A$ maps the entire plane onto a single line, so different points are sent to the same image and no transformation can recover the original point.
 
**Connection between the two ways.** The two criteria are equivalent: for a square matrix, the rows are linearly dependent exactly when the determinant is zero. Both explain the same fact, so $A^{-1}$ does not exist.
