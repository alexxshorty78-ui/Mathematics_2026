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

Using the determinant,

$$
\det A=2\cdot2-4\cdot1=4-4=0.
$$

A square matrix is invertible exactly when its determinant is nonzero. Since $\det A=0$, the inverse does not exist.

The rows also show why the matrix is not invertible. The first row is twice the second row:

$$
(2,4)=2(1,2).
$$

Thus, the rows are linearly dependent. A square matrix with linearly dependent rows is singular, so it has no inverse.

