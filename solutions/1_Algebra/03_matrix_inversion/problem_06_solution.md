# Exercise 6. Solving a System Using the Inverse

## Question

Solve $Ax=b$, where

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix},\qquad
b=
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix},
$$

using $x=A^{-1}b$. Then substitute the resulting vector back into the equation and check the result.

## Solution

First find $A^{-1}$. Since

$$
\det A=2\cdot3-1\cdot1=5\neq0,
$$

the inverse exists and is

$$
A^{-1}=\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}.
$$

Then

$$
x=A^{-1}b
=\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix} =
\begin{pmatrix}
\frac85 \\
\frac95 \\
\end{pmatrix}.
$$

Check by substitution:

$$
Ax=
\begin{pmatrix}
2\cdot\frac85+\frac95 \\
\frac85+3\cdot\frac95 \\
\end{pmatrix} =
\begin{pmatrix}
\frac{16}{5}+\frac95 \\
\frac85+\frac{27}{5} \\
\end{pmatrix} =
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}
=b.
$$

Thus, the solution is the vector shown above.

