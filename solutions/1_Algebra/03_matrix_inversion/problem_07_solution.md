# Exercise 7. Inverse of a Product

## Question

For

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix},\qquad
B=
\begin{pmatrix}
2 & 0 \\
0 & 3 \\
\end{pmatrix}
$$

compute $(AB)^{-1}$ and $B^{-1}A^{-1}$. Check that the results are the same and explain the meaning of the reversed order.

## Solution

First compute

$$
AB=
\begin{pmatrix}
2 & 3 \\
0 & 3 \\
\end{pmatrix}.
$$

Its determinant is $6\neq0$, so it is invertible. Using the $2\times2$ inverse formula,

$$
(AB)^{-1}
=\frac16
\begin{pmatrix}
3 & -3 \\
0 & 2 \\
\end{pmatrix} =
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & \frac13 \\
\end{pmatrix}.
$$

The individual inverses are

$$
A^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix},\qquad
B^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & \frac13 \\
\end{pmatrix}.
$$

Therefore,

$$
B^{-1}A^{-1} =
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & \frac13 \\
\end{pmatrix}
=(AB)^{-1}.
$$

The order is reversed because $AB$ applies $B$ first and then $A$ to a vector. To undo the full transformation, undo $A$ first with $A^{-1}$, then undo $B$ with $B^{-1}$.

