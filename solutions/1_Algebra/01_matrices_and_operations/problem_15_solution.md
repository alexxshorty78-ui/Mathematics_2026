### Exercise 15. Associativity of Multiplication and Different Calculation Paths
Given

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix},\quad B=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix},\quad C=
\begin{pmatrix}
2 & 1 \\
0 & -1 \\
\end{pmatrix}.
$$

Compute $(AB)C$ and $A(BC)$. Compare the results and the number of intermediate operations. Explain what associativity of matrix multiplication means in this example.

> **Why this exercise:** reinforces associativity by comparing two mathematically equivalent calculation paths.

#### Solution

**Compute $(AB)C$.** The intermediate product is

$$
AB=
\begin{pmatrix}
5 & 2 \\
1 & 4 \\
\end{pmatrix}.
$$

Multiplication by $C$ gives

$$
(AB)C=
\begin{pmatrix}
5\cdot2+2\cdot0 & 5\cdot1+2\cdot(-1) \\
1\cdot2+4\cdot0 & 1\cdot1+4\cdot(-1) \\
\end{pmatrix}=
\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}.
$$

**Compute $A(BC)$.** The intermediate product is

$$
BC=
\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4 \\
\end{pmatrix}.
$$

Multiplication on the left by $A$ gives

$$
A(BC)=
\begin{pmatrix}
1\cdot2+2\cdot4+0\cdot(-2) & 1\cdot1+2\cdot1+0\cdot(-4) \\
0\cdot2+1\cdot4+1\cdot(-2) & 0\cdot1+1\cdot1+1\cdot(-4) \\
\end{pmatrix}=
\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}.
$$

**Operation counts.** In the standard row-by-column algorithm, multiplying an $m\times k$ matrix by a $k\times n$ matrix uses $mkn$ scalar multiplications and $mn(k-1)$ scalar additions. This count includes products involving zero.

| Product | Output size | Scalar multiplications | Scalar additions |
| --- | --- | ---: | ---: |
| $AB$ | $2\times 2$ | 12 | 8 |
| $(AB)C$ | $2\times 2$ | 8 | 4 |
| **Total for $(AB)C$** | | **20** | **12** |
| $BC$ | $3\times 2$ | 12 | 6 |
| $A(BC)$ | $2\times 2$ | 12 | 8 |
| **Total for $A(BC)$** | | **24** | **14** |

Computing $AB$ first yields four intermediate entries, while computing $BC$ first yields six. The $AB$ path requires four fewer scalar multiplications and two fewer scalar additions overall.

By associativity, changing the grouping preserves the final product when the factors $A$, $B$, and $C$ stay in the same order.
