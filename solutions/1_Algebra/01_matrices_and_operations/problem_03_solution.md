# Exercise 3. When Can Matrices Be Multiplied?

## Question

The matrix sizes are

$$
A_{2\times3},\qquad B_{3\times4},\qquad C_{4\times2},\qquad D_{2\times2}.
$$

For the products

$$
AB,\ BA,\ BC,\ CB,\ AC,\ CA,\ AD,\ DA
$$

determine whether they are defined. If so, state the size of the result. Justify each decision using the dimension compatibility condition.

## Solution

**Condition.** The product $XY$ is defined if and only if the number of columns of $X$ equals the number of rows of $Y$. In that case the result has (rows of $X$) $\times$ (columns of $Y$) entries. To test a product, the two sizes are written next to each other, for example $(2\times3)(3\times4)$: the inner numbers must be equal, and the outer numbers give the size of the result.

| Product | Sizes | Columns of first = rows of second? | Result |
|---|---|---|---|
| $AB$ | $2\times3$ and $3\times4$ | $3=3$, yes | $2\times4$ |
| $BA$ | $3\times4$ and $2\times3$ | $4\neq2$, no | not defined |
| $BC$ | $3\times4$ and $4\times2$ | $4=4$, yes | $3\times2$ |
| $CB$ | $4\times2$ and $3\times4$ | $2\neq3$, no | not defined |
| $AC$ | $2\times3$ and $4\times2$ | $3\neq4$, no | not defined |
| $CA$ | $4\times2$ and $2\times3$ | $2=2$, yes | $4\times3$ |
| $AD$ | $2\times3$ and $2\times2$ | $3\neq2$, no | not defined |
| $DA$ | $2\times2$ and $2\times3$ | $2=2$, yes | $2\times3$ |

**Conclusion.** The products $AB$, $BC$, $CA$, $DA$ are defined, with sizes $2\times4$, $3\times2$, $4\times3$, $2\times3$. The other four are not defined. Note that $AB$ is defined while $BA$ is not, so the order of factors matters already at the level of sizes.
