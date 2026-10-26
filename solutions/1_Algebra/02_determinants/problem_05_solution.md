# Exercise 5. Row Operations

## Question

For

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2 \\
\end{pmatrix}
$$

find $\det A$ by simplifying the matrix with row operations. At each step, indicate whether and how the determinant changes.

## Solution

Use row replacements that add a multiple of one row to another. Each such replacement leaves the determinant unchanged.

First apply $R_2\leftarrow R_2-2R_1$ and $R_3\leftarrow R_3+R_1$:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 6 & 5 \\
\end{pmatrix}
$$

Both operations preserve the determinant. Next apply $R_3\leftarrow R_3+2R_2$, using the current second row:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 0 & -7 \\
\end{pmatrix}
$$

This operation also preserves the determinant. The resulting matrix is upper triangular, so

$$
\det A=1\cdot(-3)\cdot(-7)=21.
$$