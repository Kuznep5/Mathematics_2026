## Exercise 3. When Can Matrices Be Multiplied?

Given the matrix dimensions:

$$
A:2\times3,\qquad
B:3\times4,\qquad
C:4\times2,\qquad
D:2\times2.
$$

### Multiplication Rule

Two matrices can be multiplied if the number of columns in the first matrix equals the number of rows in the second matrix.

For matrices of dimensions \(m\times n\) and \(p\times q\), multiplication is possible if:

$$
\boxed{n=p}
$$

The resulting matrix has dimensions:

$$
\boxed{m\times q}
$$

### 1. Product \(AB\)

$$
(2\times3)(3\times4)
$$

The inner dimensions are equal: \(3=3\).

Therefore, multiplication is defined, and the result has dimensions:

$$
\boxed{AB:2\times4}
$$

### 2. Product \(BA\)

$$
(3\times4)(2\times3)
$$

The inner dimensions are different: \(4\neq2\).

Therefore:

$$
\boxed{BA\text{ is not defined}}
$$

### 3. Product \(BC\)

$$
(3\times4)(4\times2)
$$

The inner dimensions are equal: \(4=4\).

Therefore:

$$
\boxed{BC:3\times2}
$$

### 4. Product \(CB\)

$$
(4\times2)(3\times4)
$$

The inner dimensions are different: \(2\neq3\).

Therefore:

$$
\boxed{CB\text{ is not defined}}
$$

### 5. Product \(AC\)

$$
(2\times3)(4\times2)
$$

The inner dimensions are different: \(3\neq4\).

Therefore:

$$
\boxed{AC\text{ is not defined}}
$$

### 6. Product \(CA\)

$$
(4\times2)(2\times3)
$$

The inner dimensions are equal: \(2=2\).

Therefore:

$$
\boxed{CA:4\times3}
$$

### 7. Product \(AD\)

$$
(2\times3)(2\times2)
$$

The inner dimensions are different: \(3\neq2\).

Therefore:

$$
\boxed{AD\text{ is not defined}}
$$

### 8. Product \(DA\)

$$
(2\times2)(2\times3)
$$

The inner dimensions are equal: \(2=2\).

Therefore:

$$
\boxed{DA:2\times3}
$$

### Summary

| Product | Dimensions               | Defined? | Result dimensions |
| ------- | ------------------------ | -------- | ----------------- |
| \(AB\)  | \((2\times3)(3\times4)\) | Yes      | \(2\times4\)      |
| \(BA\)  | \((3\times4)(2\times3)\) | No       | —                 |
| \(BC\)  | \((3\times4)(4\times2)\) | Yes      | \(3\times2\)      |
| \(CB\)  | \((4\times2)(3\times4)\) | No       | —                 |
| \(AC\)  | \((2\times3)(4\times2)\) | No       | —                 |
| \(CA\)  | \((4\times2)(2\times3)\) | Yes      | \(4\times3\)      |
| \(AD\)  | \((2\times3)(2\times2)\) | No       | —                 |
| \(DA\)  | \((2\times2)(2\times3)\) | Yes      | \(2\times3\)      |

### Conclusion

Matrix multiplication is defined only when the number of columns in the first matrix equals the number of rows in the second matrix. The dimensions of the result are determined by the number of rows in the first matrix and the number of columns in the second matrix.
