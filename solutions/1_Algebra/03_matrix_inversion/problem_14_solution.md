# Exercise 14. A Matrix That Is Its Own Inverse

## Question

Assume that a square matrix $A$ satisfies

$$
A^2=I.
$$

Show that

$$
A^{-1}=A.
$$

Then give an example of a $2\times2$ matrix different from $I$ and $-I$ that satisfies this condition, and verify it by multiplication.

## Solution

Since $A^2=I$, multiplying $A$ by itself gives the identity on either side. Thus $A$ satisfies the definition of its own inverse, so $A^{-1}=A$.

For example, the matrix

$$
P=
\begin{pmatrix}
0 & 1 \\
1 & 0 \\
\end{pmatrix}
$$

swaps the two coordinates. Its off-diagonal entries show that $P\neq I$ and $P\neq -I$. Direct multiplication gives

$$
P^2=
\begin{pmatrix}
0 & 1 \\
1 & 0 \\
\end{pmatrix}
\begin{pmatrix}
0 & 1 \\
1 & 0 \\
\end{pmatrix} =
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I.
$$
