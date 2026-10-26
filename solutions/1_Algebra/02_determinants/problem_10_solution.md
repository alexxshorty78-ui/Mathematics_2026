# Exercise 10. Detecting Dependence

## Question

Without carrying out a full determinant calculation, explain why

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5 \\
\end{pmatrix}=0.
$$

Identify a specific dependence between the rows and connect it with noninvertibility of the matrix.

## Solution

The second row is twice the first row:

$$
(2,4,6)=2(1,2,3).
$$

Therefore, the rows are linearly dependent. A matrix with linearly dependent rows has determinant zero, so

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5 \\
\end{pmatrix}=0.
$$

Since the determinant is zero, the matrix is singular and is not invertible.