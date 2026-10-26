# Exercise 9. Matrix Equation

## Question

Given

$$
A=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},\qquad
B=
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix},
$$

solve $AX=B$ for $X$. Before calculating, decide on which side of the equation $A^{-1}$ must be used. Then check the result by computing $AX$.

## Solution

Since $A$ multiplies $X$ on the left, multiply both sides on the left by $A^{-1}$:

$$
A^{-1}AX=A^{-1}B.
$$

The inverse is

$$
A^{-1}=
\begin{pmatrix}
1 & -2 \\
0 & 1 \\
\end{pmatrix}.
$$

Because $A^{-1}A=I$, the equation becomes

$$
X=A^{-1}B =
\begin{pmatrix}
1 & -2 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix} =
\begin{pmatrix}
-1 & -7 \\
2 & 4 \\
\end{pmatrix}.
$$

Check by multiplying on the left by $A$:

$$
AX=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
-1 & -7 \\
2 & 4 \\
\end{pmatrix} =
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}
=B.
$$

Therefore, $X$ is the matrix shown above.

