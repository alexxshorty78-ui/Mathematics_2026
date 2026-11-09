# Exercise 11. Shortening the Calculation with Row Operations

## Question

Compute

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6 \\
\end{pmatrix}
$$

by first performing row operations that create as many zeros as possible. State which operations do not change the determinant.

## Solution

Let $A$ denote the given matrix. Adding a multiple of one row to a different row preserves the determinant.

Subtract the first row from the second and third rows.

$$
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6 \\
\end{pmatrix}
\xrightarrow{R_2\leftarrow R_2-R_1,\ R_3\leftarrow R_3-R_1}
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 2 & 3 \\
\end{pmatrix}.
$$

Then use the second row to eliminate the entry below its pivot.

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 2 & 3 \\
\end{pmatrix}
\xrightarrow{R_3\leftarrow R_3-2R_2}
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{pmatrix}.
$$

Subtract three times the third row from the first row and subtract the third row from the second row. Subtracting twice the resulting second row from the first row clears the last off-diagonal entry.

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{pmatrix}
\xrightarrow{R_1\leftarrow R_1-3R_3,\ R_2\leftarrow R_2-R_3}
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{pmatrix}
\xrightarrow{R_1\leftarrow R_1-2R_2}
I_3.
$$

Every operation was a row replacement, so $\det A=\det I_3=1$.
