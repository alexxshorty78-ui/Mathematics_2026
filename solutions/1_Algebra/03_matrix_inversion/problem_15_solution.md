# Exercise 15. Two Methods for Solving the Same System

## Question

For

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix},\qquad b=
\begin{pmatrix}
7 \\
8 \\
\end{pmatrix}
$$

solve $Ax=b$ using both methods below.

1. Use $A^{-1}b$.
2. Use Gaussian elimination.

Compare both solutions, the number of essential steps, and state which method was simpler in this example.

## Solution

### Inverse matrix method

The determinant is $\det A=2\cdot3-1\cdot1=5$. The inverse formula and the product with $b$ give

$$
A^{-1}=\frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix},
\qquad
x=A^{-1}b=\frac{1}{5}
\begin{pmatrix}
3\cdot7-8 \\
-7+2\cdot8 \\
\end{pmatrix} =
\begin{pmatrix}
\frac{13}{5} \\
\frac{9}{5} \\
\end{pmatrix}.
$$

### Gaussian elimination

Apply $R_2\leftarrow R_2-\frac{1}{2} R_1$ to the augmented matrix.

$$
\begin{pmatrix}
2 & 1 & \mid & 7 \\
1 & 3 & \mid & 8 \\
\end{pmatrix}
\longrightarrow
\begin{pmatrix}
2 & 1 & \mid & 7 \\
0 & \frac{5}{2} & \mid & \frac{9}{2} \\
\end{pmatrix}.
$$

The second row gives $x_2=\frac{9}{5}$. Back-substitution in the first row gives

$$
x_1=\frac{7-\frac{9}{5}}{2}=\frac{13}{5}.
$$

Both methods give the same solution. Substitution checks both original equations.

$$
2\cdot\frac{13}{5}+\frac{9}{5}=7,
\qquad
\frac{13}{5}+3\cdot\frac{9}{5}=8.
$$

The inverse method takes three main steps to compute the determinant, form the inverse, and multiply by $b$. Elimination also takes three main steps to perform one row replacement, solve for $x_2$, and substitute back for $x_1$. Elimination is simpler here because a single row replacement suffices and the full inverse is unnecessary.
