# Exercise 13. Undoing a Composite Transformation

## Question

The matrices

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix},\qquad H=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
$$

describe nonuniform scaling and shear. For $T=HS$, find $T^{-1}$ using both methods below.

1. Compute $T$, then find its inverse.
2. Use $(HS)^{-1}=S^{-1}H^{-1}$.

Compare the results. Additionally compute $H^{-1}S^{-1}$ and verify that the incorrect order gives a different matrix. Explain why undoing a composition requires reversing the order of the operations.

## Solution

### Invert the product directly

Multiplying $H$ by $S$ gives

$$
T=HS=
\begin{pmatrix}
2 & 1 \\
0 & 1 \\
\end{pmatrix}.
$$

Since $\det T=2$, the $2\times2$ inverse formula yields

$$
T^{-1}=\frac{1}{2}
\begin{pmatrix}
1 & -1 \\
0 & 2 \\
\end{pmatrix} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1 \\
\end{pmatrix}.
$$

### Multiply the individual inverses

The inverses of the scaling and shear are

$$
S^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1 \\
\end{pmatrix},
\qquad
H^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}.
$$

Multiplying in reverse order gives

$$
S^{-1}H^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1 \\
\end{pmatrix},
$$

which agrees with the direct result. The other order gives

$$
H^{-1}S^{-1}=
\begin{pmatrix}
\frac{1}{2} & -1 \\
0 & 1 \\
\end{pmatrix}.
$$

The two products differ in the upper-right entry. The transformation $HS$ scales first and shears second. Its inverse undoes the shear first with $H^{-1}$, then undoes the scaling with $S^{-1}$.
