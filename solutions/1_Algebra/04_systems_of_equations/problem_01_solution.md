# Exercise 1. From a System to a Matrix

## Question

Write the system

$$
\begin{cases}
2x-y+z=4, \\
x+3y-2z=1, \\
3x+y+z=7.
\end{cases}
$$

in the form $Ax=b$.
Identify the coefficient matrix, the vector of unknowns, and the right-hand side vector. Explain how each row of the matrix corresponds to one equation.

## Solution

Let $\mathbf{x}$ denote the vector of unknowns, so that it is distinct from the scalar variable $x$. The matrix form is

$$
A\mathbf{x}=\mathbf{b},
\qquad
A=\begin{pmatrix}2&-1&1\\1&3&-2\\3&1&1\end{pmatrix},
\quad
\mathbf{x}=\begin{pmatrix}x\\y\\z\end{pmatrix},
\quad
\mathbf{b}=\begin{pmatrix}4\\1\\7\end{pmatrix}.
$$

The columns of $A$ contain the coefficients of $x$, $y$, and $z$, in that order. Multiplication gives

$$
A\mathbf{x}=
\begin{pmatrix}2x-y+z\\x+3y-2z\\3x+y+z\end{pmatrix}
=
\begin{pmatrix}4\\1\\7\end{pmatrix}.
$$

Thus the first row represents $2x-y+z=4$, the second represents $x+3y-2z=1$, and the third represents $3x+y+z=7$.
