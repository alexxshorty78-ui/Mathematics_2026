### Exercise 2. Addition and Scalar Multiplication

For

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

compute

$$
A+B,\qquad A-B,\qquad 3A-2B.
$$

Explain why matrix addition is possible only for matrices of the same size.

> **Why this exercise:** reinforces entry-by-entry operations and the importance of compatible dimensions.

#### Solution

**Sum $A+B$**

Add corresponding entries:

$$
A+B=
\begin{pmatrix}
1+4 & 2+(-2) \\
-1+0 & 3+5 \\
\end{pmatrix}
$$

Hence

$$
A+B=
\begin{pmatrix}
5 & 0 \\
-1 & 8 \\
\end{pmatrix}
$$

**Difference $A-B$**

Subtract corresponding entries:

$$
A-B=
\begin{pmatrix}
1-4 & 2-(-2) \\
-1-0 & 3-5 \\
\end{pmatrix}
$$

Hence

$$
A-B=
\begin{pmatrix}
-3 & 4 \\
-1 & -2 \\
\end{pmatrix}
$$

**Linear combination $3A-2B$**

First compute the scalar multiples:

$$
3A=
\begin{pmatrix}
3 & 6 \\
-3 & 9 \\
\end{pmatrix},\qquad 2B=
\begin{pmatrix}
8 & -4 \\
0 & 10 \\
\end{pmatrix}
$$

Then subtract entry by entry:

$$
3A-2B=
\begin{pmatrix}
3-8 & 6-(-4) \\
-3-0 & 9-10 \\
\end{pmatrix}
$$

Hence

$$
3A-2B=
\begin{pmatrix}
-5 & 10 \\
-3 & -1 \\
\end{pmatrix}
$$

**Why the sizes must agree**

Matrix addition is defined entry by entry: the $(i,j)$ entry of $A+B$ is $a_{ij}+b_{ij}$. This requires that every position $(i,j)$ of $A$ has a corresponding position $(i,j)$ in $B$.

If $A$ is of size $m\times n$ and $B$ is of size $p\times q$, then the entries correspond for all positions only when $m=p$ and $n=q$. Otherwise some entry of one matrix has no partner in the other, and the sum is not defined. For example, a $2\times 2$ matrix and a $2\times 3$ matrix cannot be added, because the third column has nothing to be added to.

The same condition applies to subtraction and to any linear combination such as $3A-2B$, while multiplication by a scalar is always defined, since it acts on each entry separately.