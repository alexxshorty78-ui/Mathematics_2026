# Exercise 15. Combining Determinant Properties

## Question

Let $A$ and $B$ be invertible $2\times2$ matrices with

$$
\det A=-2,\qquad \det B=3.
$$

Without finding the entries of the matrices, compute

$$
\det\left(B^{-1}A^TB\right).
$$

State the determinant properties you use in order and explain why the factors involving $B$ eventually cancel.

## Solution

First apply multiplicativity of the determinant.

$$
\det(B^{-1}A^TB)=\det(B^{-1})\det(A^T)\det B.
$$

The determinant of an inverse is the reciprocal of the original determinant, and transposition preserves the determinant. Therefore,

$$
\det(B^{-1}A^TB)
=\frac{1}{\det B}\,(\det A)\,\det B
=\frac{1}{3}\cdot(-2)\cdot3
=-2.
$$

The factors involving $B$ cancel because $\det B\neq 0$ and $\det(B^{-1})\det B=1$.
