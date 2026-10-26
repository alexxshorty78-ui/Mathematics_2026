# Exercise 8. Inverse of a Transformation

## Question

The matrix

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & \frac12 \\
\end{pmatrix}
$$

describes a scaling of the plane. Find $S^{-1}$ and explain geometrically what the inverse transformation does. Check the action of the pair $S,S^{-1}$ on one simple vector.

## Solution

The matrix $S$ scales the first coordinate by $2$ and the second coordinate by $\frac12$. Its inverse undoes both changes:

$$
S^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & 2 \\
\end{pmatrix}.
$$

Indeed,

$$
SS^{-1}=S^{-1}S=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I.
$$

Geometrically, $S^{-1}$ contracts the first coordinate by $\frac12$ and stretches the second coordinate by $2$.

For example, let

$$
v=
\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}.
$$

Then

$$
Sv=
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix},\qquad
S^{-1}(Sv)=
\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}
=v.
$$

Thus, applying $S^{-1}$ after $S$ returns the original vector.

