### Exercise 3. When Does the Inverse Not Exist?
 
#### Solution
 
**Using the determinant.**
 
$$
\det A = 2\cdot2-4\cdot1 = 0.
$$
 
A square matrix is invertible if and only if its determinant is nonzero, so $A^{-1}$ does not exist.
 
**Using dependence between the rows.** The first row is twice the second row:
 
$$
(2,\ 4) = 2\cdot(1,\ 2).
$$
 
The rows are linearly dependent, so the rank of $A$ is $1<2$. A $2\times2$ matrix with rank less than $2$ is not invertible. Geometrically, $A$ maps the whole plane onto a single line, so the map cannot be undone.
 
The two criteria agree: dependent rows give $\det A=0$, and $\det A=0$ means the rows are dependent.
