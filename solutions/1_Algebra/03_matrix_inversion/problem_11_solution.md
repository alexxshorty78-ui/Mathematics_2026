# Exercise 11. Parameter and Invertibility

## Question

For

$$
A(t)=
\begin{pmatrix}
1 & t \\
t & 1 \\
\end{pmatrix}
$$

find all $t$ for which the matrix is invertible, and then give a formula for $A(t)^{-1}$. Explain what happens to this formula at the excluded values.

## Solution

The determinant determines invertibility.

$$
\det A(t)=1-t^2=(1-t)(1+t).
$$

For real $t$, the inverse exists exactly when $t\neq1$ and $t\neq-1$. The $2\times2$ inverse formula gives

$$
A(t)^{-1}=\frac{1}{1-t^2}
\begin{pmatrix}
1 & -t \\
-t & 1 \\
\end{pmatrix}.
$$

At $t=1$ the rows are equal, and at $t=-1$ the rows are negatives of each other. The matrix is singular in both cases, and the denominator in the formula is zero.
