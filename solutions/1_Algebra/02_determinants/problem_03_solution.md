# Exercise 3. Swapping Two Rows

## Question

For

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 3 & 1 \\
2 & 1 & 1 \\
\end{pmatrix}
$$

compute $\det A$. Form $B$ by swapping the first and second rows of $A$. First predict $\det B$ using a determinant property, then verify the prediction by calculation.

## Solution

Expanding $\det A$ along the first row,

$$
\det A=1(3\cdot1-1\cdot1)-2(0\cdot1-1\cdot2)=2+4=6.
$$

Swapping two rows changes the sign of the determinant. Therefore, the predicted value is

$$
\det B=-\det A=-6.
$$

The matrix formed by the row swap is

$$
B=
\begin{pmatrix}
0 & 3 & 1 \\
1 & 2 & 0 \\
2 & 1 & 1 \\
\end{pmatrix}.
$$

Expanding along the first row verifies the prediction:

$$
\det B=-3(1\cdot1-0\cdot2)+1(1\cdot1-2\cdot2)=-3-3=-6.
$$