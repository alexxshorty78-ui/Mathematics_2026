### Exercise 5. Matrix Times Vector

Let

$$
A=
\begin{pmatrix}
2 & -1 \\
1 & 3 \\
\end{pmatrix},\qquad x=
\begin{pmatrix}
4 \\
2 \\
\end{pmatrix}.
$$

Compute $Ax$. Then express $Ax$ as a linear combination of the columns of $A$, with coefficients coming from the vector $x$.

> **Why this exercise:** shows that multiplying a matrix by a vector can be understood as a linear combination of the matrix columns.

#### Solution

The matrix $A$ is of size $2\times2$ and the vector $x$ is of size $2\times1$. The inner dimensions agree, so $Ax$ is defined and has size $2\times1$.

**Row-wise computation**

Each entry of $Ax$ is the sum of products of a row of $A$ with the entries of $x$:

$$
Ax=
\begin{pmatrix}
2\cdot4+(-1)\cdot2 \\
1\cdot4+3\cdot2 \\
\end{pmatrix}
$$

Hence

$$
Ax=
\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}
$$

**Column-wise interpretation**

Denote the columns of $A$ by

$$
a_1=
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix},\qquad a_2=
\begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}.
$$

The coefficients are the entries of $x$, namely $x_1=4$ and $x_2=2$. Then

$$
Ax = x_1a_1+x_2a_2 = 4a_1+2a_2.
$$

Written out in full:

$$
Ax=4
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}
+2
\begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}
$$

Computing the scalar multiples gives

$$
Ax=
\begin{pmatrix}
8 \\
4 \\
\end{pmatrix}
+
\begin{pmatrix}
-2 \\
6 \\
\end{pmatrix}
$$

Hence

$$
Ax=
\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}
$$

**Conclusion**

Both methods give the same result. The product $Ax$ is the linear combination of the columns of $A$ in which the first column is taken with coefficient $4$ and the second column with coefficient $2$. In general, for an $m\times n$ matrix $A$ with columns $a_1,\dots,a_n$ and a vector $x$ with entries $x_1,\dots,x_n$,

$$
Ax = x_1a_1+x_2a_2+\dots+x_na_n.
$$

Consequently, $Ax$ always lies in the span of the columns of $A$.S