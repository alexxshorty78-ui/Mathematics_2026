### Exercise 4. Matrix Multiplication and Noncommutativity

For

$$
A=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix}
$$

compute $AB$ and $BA$. Is $AB=BA$? Use this example to explain what noncommutativity of matrix multiplication means.

> **Why this exercise:** shows one of the most important differences between matrix multiplication and multiplication of numbers.

#### Solution

Both matrices are of size $2\times2$, so both products $AB$ and $BA$ are defined and have size $2\times2$. The $(i,j)$ entry of a product is the sum of products of the entries in row $i$ of the first factor with the corresponding entries in column $j$ of the second factor.

**Product $AB$**

$$
AB=
\begin{pmatrix}
1\cdot2+2\cdot3 & 1\cdot0+2\cdot1 \\
0\cdot2+1\cdot3 & 0\cdot0+1\cdot1 \\
\end{pmatrix}
$$

Hence

$$
AB=
\begin{pmatrix}
8 & 2 \\
3 & 1 \\
\end{pmatrix}
$$

**Product $BA$**

$$
BA=
\begin{pmatrix}
2\cdot1+0\cdot0 & 2\cdot2+0\cdot1 \\
3\cdot1+1\cdot0 & 3\cdot2+1\cdot1 \\
\end{pmatrix}
$$

Hence

$$
BA=
\begin{pmatrix}
2 & 4 \\
3 & 7 \\
\end{pmatrix}
$$

**Comparison**

The matrices $AB$ and $BA$ are different, for example their $(1,1)$ entries are $8$ and $2$. Therefore

$$
AB\neq BA.
$$

**Meaning of noncommutativity**

Matrix multiplication is called noncommutative because the order of the factors matters: in general $AB\neq BA$. For real numbers $a$ and $b$ the equality $ab=ba$ always holds, but this property does not carry over to matrices.

In this example both products exist and have the same size, yet they differ. This shows that the failure of commutativity is not only a matter of dimensions (as in Exercise 3, where $AB$ could exist while $BA$ did not), but occurs even for square matrices of the same size.

Consequently, the expressions "multiply $A$ by $B$ on the right" and "multiply $A$ by $B$ on the left" describe different operations. A single example with $AB\neq BA$ is enough to show that commutativity does not hold in general. It does not exclude that some particular pairs of matrices satisfy $AB=BA$.S