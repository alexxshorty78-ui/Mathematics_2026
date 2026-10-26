# Exercise 2. Determinant of a 3×3 Matrix

## Question

For

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
2 & 1 & 5 \\
\end{pmatrix}
$$

compute $\det A$ using Sarrus' rule. Then perform one simple check using a property of the determinant.

## Solution

### Sarrus' rule

The sum of the downward diagonal products is

$$
1\cdot3\cdot5+2\cdot4\cdot2+(-1)\cdot0\cdot1=15+16+0=31.
$$

The sum of the upward diagonal products is

$$
(-1)\cdot3\cdot2+2\cdot0\cdot5+1\cdot4\cdot1=-6+0+4=-2.
$$

Therefore,

$$
\det A=31-(-2)=33.
$$

### Check using a row operation

Apply $R_3\leftarrow R_3-2R_1$. Adding a multiple of one row to another does not change the determinant. The resulting matrix is

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & -3 & 7 \\
\end{pmatrix}.
$$

Expanding along the first column gives

$$
\det A=1\bigl(3\cdot7-4\cdot(-3)\bigr)=21+12=33.
$$

The check agrees with Sarrus' rule.