### Exercise 7. Identity Matrix, Zero Matrix, and Powers

Given

$$
A=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

#### 1. Computations

**Calculation of $AI$ and $IA$**

Using $I = \begin{pmatrix} 1 & 0 \\ 0 & 1 \\ \end{pmatrix}$:

$$
AI=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=
\begin{pmatrix}
2\cdot1 + 1\cdot0 & 2\cdot0 + 1\cdot1 \\
0\cdot1 + 2\cdot0 & 0\cdot0 + 2\cdot1 \\
\end{pmatrix}
=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

$$
IA=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
=
\begin{pmatrix}
1\cdot2 + 0\cdot0 & 1\cdot1 + 0\cdot2 \\
0\cdot2 + 1\cdot0 & 0\cdot1 + 1\cdot2 \\
\end{pmatrix}
=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

**Calculation of $A+0$**

Using $0 = \begin{pmatrix} 0 & 0 \\ 0 & 0 \\ \end{pmatrix}$:

$$
A+0=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
+
\begin{pmatrix}
0 & 0 \\
0 & 0 \\
\end{pmatrix}
=
\begin{pmatrix}
2+0 & 1+0 \\
0+0 & 2+0 \\
\end{pmatrix}
=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

**Calculation of $A^2$**

$$
A^2=
AA=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
=
\begin{pmatrix}
2\cdot2 + 1\cdot0 & 2\cdot1 + 1\cdot2 \\
0\cdot2 + 2\cdot0 & 0\cdot1 + 2\cdot2 \\
\end{pmatrix}
=
\begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix}
$$

**Calculation of $A^3$**

$$
A^3=
A^2 A=
\begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
=
\begin{pmatrix}
4\cdot2 + 4\cdot0 & 4\cdot1 + 4\cdot2 \\
0\cdot2 + 4\cdot0 & 0\cdot1 + 4\cdot2 \\
\end{pmatrix}
=
\begin{pmatrix}
8 & 12 \\
0 & 8 \\
\end{pmatrix}
$$

#### 2. Roles of $I$ and $0$

- **Identity Matrix $I$:** Acts as the multiplicative identity element for matrix multiplication, meaning $AI = IA = A$.
- **Zero Matrix $0$:** Acts as the additive identity element for matrix addition, meaning $A + 0 = A$.

#### 3. Pattern in Successive Powers of $A$

Observing the powers of $A$:

$$
A^1 = 
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix},\qquad
A^2 = 
\begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix},\qquad
A^3 = 
\begin{pmatrix}
8 & 12 \\
0 & 8 \\
\end{pmatrix}
$$

The general pattern for any positive integer $k$ is given by:

$$
A^k = 
\begin{pmatrix}
2^k & k \cdot 2^{k-1} \\
0 & 2^k \\
\end{pmatrix}
$$

- The main diagonal entries are always equal to $2^k$.
- The lower-left entry remains $0$.
- The upper-right entry grows as $k \cdot 2^{k-1}$.

> **Why this exercise:** organizes the roles of neutral elements and reveals regularity in successive powers of a matrix.S