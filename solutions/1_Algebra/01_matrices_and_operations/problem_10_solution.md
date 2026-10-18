### Exercise 10. Columns of a Matrix Product

Given

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1 \\
\end{pmatrix}.
$$

Denote the columns of $B$ by $b_1,b_2$.

1. Compute $Ab_1$ and $Ab_2$.
2. Compute the matrix $AB$.
3. Compare the results and explain why the columns of $AB$ are exactly the vectors $Ab_1$ and $Ab_2$.

> **Why this exercise:** extends the interpretation of matrix-vector multiplication to a full product of two matrices instead of simply repeating another $Ax$ exercise.

#### Solution

The matrix $A$ is of size $2\times3$ and $B$ is of size $3\times2$. The inner dimensions agree, so $AB$ is defined and has size $2\times2$. The columns of $B$ are

$$
b_1=
\begin{pmatrix}
1 \\
-1 \\
3 \\
\end{pmatrix},\qquad b_2=
\begin{pmatrix}
2 \\
0 \\
1 \\
\end{pmatrix}.
$$

**Part 1: the products $Ab_1$ and $Ab_2$**

$$
Ab_1=
\begin{pmatrix}
1\cdot1+2\cdot(-1)+0\cdot3 \\
0\cdot1+1\cdot(-1)+1\cdot3 \\
\end{pmatrix}
$$

Hence

$$
Ab_1=
\begin{pmatrix}
-1 \\
2 \\
\end{pmatrix}
$$

Similarly,

$$
Ab_2=
\begin{pmatrix}
1\cdot2+2\cdot0+0\cdot1 \\
0\cdot2+1\cdot0+1\cdot1 \\
\end{pmatrix}
$$

Hence

$$
Ab_2=
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}
$$

**Part 2: the product $AB$**

Each entry is the sum of products of a row of $A$ with a column of $B$:

$$
AB=
\begin{pmatrix}
1\cdot1+2\cdot(-1)+0\cdot3 & 1\cdot2+2\cdot0+0\cdot1 \\
0\cdot1+1\cdot(-1)+1\cdot3 & 0\cdot2+1\cdot0+1\cdot1 \\
\end{pmatrix}
$$

Hence

$$
AB=
\begin{pmatrix}
-1 & 2 \\
2 & 1 \\
\end{pmatrix}
$$

**Part 3: comparison and explanation**

The first column of $AB$ is $(-1,\,2)^T$, which is $Ab_1$. The second column of $AB$ is $(2,\,1)^T$, which is $Ab_2$. Therefore

$$
AB=
\begin{pmatrix}
Ab_1 & Ab_2 \\
\end{pmatrix}.
$$

The reason is visible from the definition of the product. The $(i,j)$ entry of $AB$ is

$$
(AB)_{ij}=\sum_{k=1}^{3}a_{ik}b_{kj}.
$$

For a fixed $j$, the right-hand side is the sum of products of the $i$-th row of $A$ with the entries of the $j$-th column $b_j$, which is exactly the $i$-th entry of the vector $Ab_j$. Hence the $j$-th column of $AB$ equals $Ab_j$ for every $j$. In particular, the computation of $AB$ consists of $2$ independent matrix-vector products, one for each column of $B$.

**Column interpretation**

By Exercise 5, each $Ab_j$ is a linear combination of the columns $a_1,a_2,a_3$ of $A$, with coefficients taken from $b_j$:

$$
Ab_1=1\cdot a_1-1\cdot a_2+3\cdot a_3,\qquad Ab_2=2\cdot a_1+0\cdot a_2+1\cdot a_3.
$$

Consequently, every column of $AB$ is a linear combination of the columns of $A$, and the entries of the corresponding column of $B$ are the coefficients.

**Conclusion**

The product $AB$ can be computed column by column: the $j$-th column of $AB$ is $A$ multiplied by the $j$-th column of $B$. This agrees with the direct entry-by-entry computation.