### Exercise 3. When Can Matrices Be Multiplied?
 
The sizes are $A_{2\times3}$, $B_{3\times4}$, $C_{4\times2}$, $D_{2\times2}$.
 
**Condition.** The product $XY$ is defined if and only if the number of columns of $X$ equals the number of rows of $Y$. The result has (rows of $X$) $\times$ (columns of $Y$).
 
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
 
**Conclusion.** The products $AB$, $BC$, $CA$, $DA$ are defined. Note that $AB$ is defined while $BA$ is not, so the order of factors matters already at the level of sizes.
