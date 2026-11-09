# Exercise 12. A Parameter Revealed by a Row Operation

## Question

For

$$
A(t)=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & t \\
0 & 1 & 1 \\
\end{pmatrix}
$$

find the values of $t$ for which the matrix is not invertible.

Before computing the determinant, perform the operation

$$
R_2\leftarrow R_2-2R_1
$$

and use the resulting structure. At the end, explain what special thing happens to the rows for the value of the parameter you found.

## Solution

The replacement $R_2\leftarrow R_2-2R_1$ preserves the determinant and leaves only one potentially nonzero entry in the second row.

$$
A(t)\longrightarrow
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & t-6 \\
0 & 1 & 1 \\
\end{pmatrix}.
$$

Expansion along the second row gives

$$
\det A(t)=(-1)^{2+3}(t-6)
\det\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
=6-t.
$$

The matrix is not invertible exactly when its determinant vanishes, which occurs at $t=6$. At this value the original second row is twice the first row, and the replacement turns it into a zero row.
