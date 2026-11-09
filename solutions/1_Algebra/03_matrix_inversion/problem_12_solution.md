# Exercise 12. Finding Inverses Without Starting from Scratch

## Question

It is known that

$$
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}.
$$

Without finding $A$, compute $(3A)^{-1}$, $(A^T)^{-1}$, and $(A^2)^{-1}$. Justify each result using the appropriate property.

## Solution

### Scalar multiple

Multiplying $A$ by $3$ requires multiplying its inverse by $\frac{1}{3}$, since $(3A)(\frac{1}{3} A^{-1})=I$. Thus,

$$
(3A)^{-1}=\frac{1}{3} A^{-1}
=\frac{1}{3}
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}.
$$

### Transpose

Transposing $A^{-1}A=I$ gives $A^T(A^{-1})^T=I$. Hence,

$$
(A^T)^{-1}=(A^{-1})^T =
\begin{pmatrix}
2 & -3 \\
-1 & 2 \\
\end{pmatrix}.
$$

### Square

The inverse of a product reverses the order of the factors. Here the two factors are identical, so $(A^2)^{-1}=(A^{-1})^2$.

$$
(A^2)^{-1}=
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix} =
\begin{pmatrix}
7 & -4 \\
-12 & 7 \\
\end{pmatrix}.
$$
