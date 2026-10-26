# Exercise 1. Definition of the Inverse

## Question

For

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix},\qquad
B=
\begin{pmatrix}
1 & -1 \\
-1 & 2 \\
\end{pmatrix}
$$

check, without using a formula, whether $B=A^{-1}$. Compute $AB$ and $BA$ and relate the result to the definition of the inverse.

## Solution

Compute $AB$ directly:

$$
AB=
\begin{pmatrix}
2\cdot1+1\cdot(-1) & 2\cdot(-1)+1\cdot2 \\
1\cdot1+1\cdot(-1) & 1\cdot(-1)+1\cdot2 \\
\end{pmatrix} =
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I.
$$

Now compute $BA$:

$$
BA=
\begin{pmatrix}
1\cdot2+(-1)\cdot1 & 1\cdot1+(-1)\cdot1 \\
(-1)\cdot2+2\cdot1 & (-1)\cdot1+2\cdot1 \\
\end{pmatrix} =
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I.
$$

A matrix $B$ is the inverse of $A$ when both products $AB$ and $BA$ equal the identity matrix. Since both products equal $I$, $B=A^{-1}$.

