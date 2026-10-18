### Exercise 2. Addition and Scalar Multiplication

Given

$$
A=
\begin{pmatrix}
1 & 2 \\
-1 & 3 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
4 & -2 \\
0 & 5 \\
\end{pmatrix}
$$

#### 1. Computation of $A+B$

$$
A+B=
\begin{pmatrix}
1+4 & 2+(-2) \\
-1+0 & 3+5 \\
\end{pmatrix}
=
\begin{pmatrix}
5 & 0 \\
-1 & 8 \\
\end{pmatrix}
$$

#### 2. Computation of $A-B$

$$
A-B=
\begin{pmatrix}
1-4 & 2-(-2) \\
-1-0 & 3-5 \\
\end{pmatrix}
=
\begin{pmatrix}
-3 & 4 \\
-1 & -2 \\
\end{pmatrix}
$$

#### 3. Computation of $3A-2B$

$$
3A-2B=
3
\begin{pmatrix}
1 & 2 \\
-1 & 3 \\
\end{pmatrix}
-
2
\begin{pmatrix}
4 & -2 \\
0 & 5 \\
\end{pmatrix}
$$

$$
3A-2B=
\begin{pmatrix}
3 & 6 \\
-3 & 9 \\
\end{pmatrix}
-
\begin{pmatrix}
8 & -4 \\
0 & 10 \\
\end{pmatrix}
=
\begin{pmatrix}
-5 & 10 \\
-3 & -1 \\
\end{pmatrix}
$$

#### Explanation

Matrix addition is defined entry-by-entry, where the entry in position $(i, j)$ of the sum matrix is obtained by adding the corresponding entry $(i, j)$ of the first matrix to the entry $(i, j)$ of the second matrix. For this operation to be well-defined, every position in the first matrix must correspond uniquely to an entry in the same position in the second matrix. Consequently, matrix addition is possible only for matrices of the exact same size.

> **Why this exercise:** reinforces entry-by-entry operations and the importance of compatible dimensions.