# Exercise 3. Swapping Two Rows

## Question

For

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 3 & 1 \\
2 & 1 & 1 \\
\end{pmatrix}
$$

compute $\det A$. Then form a matrix $B$ by swapping the first and second rows of $A$. First predict $\det B$ using a determinant property, and then verify your prediction by calculation.

## Solution

### Given

The matrix $A$ from the Question, and $B$ obtained from $A$ by swapping $R_1$ and $R_2$.

### Find

The value $\det A$, a predicted value of $\det B$, and a verification of the prediction.

### Method and steps

*Step 1. Compute $\det A$ by Sarrus' rule.* The plus terms are $1\cdot3\cdot1=3$, $2\cdot1\cdot2=4$ and $0\cdot0\cdot1=0$. The minus terms are $0\cdot3\cdot2=0$, $1\cdot1\cdot1=1$ and $2\cdot0\cdot1=0$. Hence

$$
\det A = (3+4+0)-(0+1+0) = 7-1 = 6.
$$

*Step 2. Write down $B$.*

$$
B=
\begin{pmatrix}
0 & 3 & 1 \\
1 & 2 & 0 \\
2 & 1 & 1 \\
\end{pmatrix}.
$$

*Step 3. Predict $\det B$.* Swapping two rows multiplies the determinant by $-1$. Therefore

$$
\det B = -\det A = -6.
$$

*Step 4. Verify by Sarrus' rule.* The plus terms are $0\cdot2\cdot1=0$, $3\cdot0\cdot2=0$ and $1\cdot1\cdot1=1$. The minus terms are $1\cdot2\cdot2=4$, $0\cdot0\cdot1=0$ and $3\cdot1\cdot1=3$. Hence

$$
\det B = (0+0+1)-(4+0+3) = 1-7 = -6.
$$

The calculation confirms the prediction.

### Answer

$\det A=6$, predicted $\det B=-6$, verified $\det B=-6$.
