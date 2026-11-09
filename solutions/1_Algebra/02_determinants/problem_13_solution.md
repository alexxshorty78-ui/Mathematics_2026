# Exercise 13. Determinant by Elimination

## Question

Compute the determinant

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2 \\
\end{pmatrix}
$$

using elimination. Record the effect of every row operation used on the value of the determinant.

## Solution

Use $R_2\leftarrow R_2-2R_1$ and $R_3\leftarrow R_3-R_1$ to clear the entries below the first pivot.

$$
A\longrightarrow
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & -2 & -1 \\
\end{pmatrix}.
$$

Each of these two row replacements leaves the determinant unchanged. The replacement $R_3\leftarrow R_3+2R_2$ also leaves the determinant unchanged and gives an upper triangular matrix.

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{pmatrix}.
$$

Its determinant is the product of the diagonal entries, so $\det A=1\cdot1\cdot1=1$.
