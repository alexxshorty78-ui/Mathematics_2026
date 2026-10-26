# Exercise 2. Formula for a 2×2 Matrix

## Question

Find the inverse of

$$
A=
\begin{pmatrix}
3 & 2 \\
5 & 4 \\
\end{pmatrix}
$$

using the formula for a $2\times2$ matrix. At the end, check the result by computing one product with $A$.

## Solution

For a general $2\times2$ matrix, write

$$
M=
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}.
$$

Its determinant is $ad-bc$. If this value is nonzero, its inverse is found by swapping the diagonal entries, changing the signs of the off-diagonal entries, and dividing by the determinant:

$$
M^{-1}=\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a \\
\end{pmatrix}.
$$

For the given matrix $A$,

$$
\det A=3\cdot4-2\cdot5=12-10=2\neq0.
$$

Therefore,

$$
A^{-1}=\frac{1}{2}
\begin{pmatrix}
4 & -2 \\
-5 & 3 \\
\end{pmatrix} =
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2} \\
\end{pmatrix}.
$$

Check by multiplying $A$ by the proposed inverse:

$$
AA^{-1}=
\begin{pmatrix}
3\cdot2+2\cdot\left(-\frac{5}{2}\right) & 3\cdot(-1)+2\cdot\frac{3}{2} \\
5\cdot2+4\cdot\left(-\frac{5}{2}\right) & 5\cdot(-1)+4\cdot\frac{3}{2} \\
\end{pmatrix} =
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I.
$$

The product is the identity, so the computed matrix is the inverse of $A$.

