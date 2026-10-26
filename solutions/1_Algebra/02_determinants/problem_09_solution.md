# Exercise 9. Area and the Determinant

## Question

The vectors

$$
u=
\begin{pmatrix}
3 \\
1 \\
\end{pmatrix},\qquad
v=
\begin{pmatrix}
1 \\
4 \\
\end{pmatrix}
$$

span a parallelogram. Compute its area using a determinant. Then reverse the order of the vectors and explain what changes in the determinant and what does not change in the area.

## Solution

Place $u$ and $v$ as the columns of a matrix:

$$
\begin{pmatrix}
3 & 1 \\
1 & 4 \\
\end{pmatrix}.
$$

Its determinant is

$$
3\cdot4-1\cdot1=11.
$$

The parallelogram's area is the absolute value of this determinant, so the area is $|11|=11$ square units.

Reversing the order of the vectors swaps the columns:

$$
\begin{pmatrix}
1 & 3 \\
4 & 1 \\
\end{pmatrix}.
$$

The new determinant is

$$
1\cdot1-3\cdot4=-11.
$$

Its sign changes, but its absolute value remains $11$, so the area does not change.