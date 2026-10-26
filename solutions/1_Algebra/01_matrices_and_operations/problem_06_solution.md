### Exercise 6. Transpose

For

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix}
$$

compute $A^T$, $B^T$, and $AB$. Then verify in this example that

$$
(AB)^T=B^TA^T.
$$

> **Why this exercise:** teaches transposition and an important property that reverses the order of factors.

#### Solution

The transpose of a matrix is obtained by writing its rows as columns. The matrix $A$ is of size $2\times3$, so $A^T$ is of size $3\times2$. The matrix $B$ is of size $3\times2$, so $B^T$ is of size $2\times3$.

**Transposes**

$$
A^T=
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6 \\
\end{pmatrix}
$$

$$
B^T=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3 \\
\end{pmatrix}
$$

**Product $AB$**

The inner dimensions are $3$ and $3$, so $AB$ is defined and has size $2\times2$.

$$
AB=
\begin{pmatrix}
1\cdot1+2\cdot2+3\cdot(-1) & 1\cdot0+2\cdot1+3\cdot3 \\
4\cdot1+5\cdot2+6\cdot(-1) & 4\cdot0+5\cdot1+6\cdot3 \\
\end{pmatrix}
$$

Hence

$$
AB=
\begin{pmatrix}
2 & 11 \\
8 & 23 \\
\end{pmatrix}
$$

**Left-hand side $(AB)^T$**

$$
(AB)^T=
\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}
$$

**Right-hand side $B^TA^T$**

The matrix $B^T$ is of size $2\times3$ and $A^T$ is of size $3\times2$, so the product is defined and has size $2\times2$.

$$
B^TA^T=
\begin{pmatrix}
1\cdot1+2\cdot2+(-1)\cdot3 & 1\cdot4+2\cdot5+(-1)\cdot6 \\
0\cdot1+1\cdot2+3\cdot3 & 0\cdot4+1\cdot5+3\cdot6 \\
\end{pmatrix}
$$

Hence

$$
B^TA^T=
\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}
$$

**Conclusion**

The matrices $(AB)^T$ and $B^TA^T$ are equal, so in this example

$$
(AB)^T=B^TA^T.
$$

The product $A^TB^T$ is defined: $A^T$ has size $3\times2$ and $B^T$ has size $2\times3$, so $A^TB^T$ has size $3\times3$. This differs in size from $(AB)^T$, which has size $2\times2$. The correct transpose identity reverses the order of the factors: $(AB)^T=B^TA^T$.