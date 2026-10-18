### Exercise 7. Identity Matrix, Zero Matrix, and Powers

For

$$
A=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

compute

$$
AI,\qquad IA,\qquad A+0,\qquad A^2,\qquad A^3.
$$

Explain the roles of the matrices $I$ and $0$, and describe the pattern you observe in successive powers of $A$.

> **Why this exercise:** organizes the roles of neutral elements and reveals regularity in successive powers of a matrix.

#### Solution

Here $I$ and $0$ denote the $2\times2$ identity matrix and the $2\times2$ zero matrix:

$$
I=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix},\qquad 0=
\begin{pmatrix}
0 & 0 \\
0 & 0 \\
\end{pmatrix}.
$$

**Product $AI$**

$$
AI=
\begin{pmatrix}
2\cdot1+1\cdot0 & 2\cdot0+1\cdot1 \\
0\cdot1+2\cdot0 & 0\cdot0+2\cdot1 \\
\end{pmatrix}
$$

Hence

$$
AI=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

**Product $IA$**

$$
IA=
\begin{pmatrix}
1\cdot2+0\cdot0 & 1\cdot1+0\cdot2 \\
0\cdot2+1\cdot0 & 0\cdot1+1\cdot2 \\
\end{pmatrix}
$$

Hence

$$
IA=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

**Sum $A+0$**

$$
A+0=
\begin{pmatrix}
2+0 & 1+0 \\
0+0 & 2+0 \\
\end{pmatrix}
$$

Hence

$$
A+0=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

**Power $A^2$**

$$
A^2=AA=
\begin{pmatrix}
2\cdot2+1\cdot0 & 2\cdot1+1\cdot2 \\
0\cdot2+2\cdot0 & 0\cdot1+2\cdot2 \\
\end{pmatrix}
$$

Hence

$$
A^2=
\begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix}
$$

**Power $A^3$**

$$
A^3=A^2A=
\begin{pmatrix}
4\cdot2+4\cdot0 & 4\cdot1+4\cdot2 \\
0\cdot2+4\cdot0 & 0\cdot1+4\cdot2 \\
\end{pmatrix}
$$

Hence

$$
A^3=
\begin{pmatrix}
8 & 12 \\
0 & 8 \\
\end{pmatrix}
$$

**Roles of $I$ and $0$**

The computation shows that $AI=IA=A$. The identity matrix $I$ is the neutral element of matrix multiplication, playing the same role as the number $1$ for multiplication of numbers. It leaves every matrix of compatible size unchanged.

The computation also shows that $A+0=A$. The zero matrix $0$ is the neutral element of matrix addition, playing the same role as the number $0$ for addition of numbers.

**Pattern in the powers**

Collecting the results:

$$
A^1=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix},\qquad A^2=
\begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix},\qquad A^3=
\begin{pmatrix}
8 & 12 \\
0 & 8 \\
\end{pmatrix}.
$$

The diagonal entries are $2$, $4$, $8$, that is $2^n$. The entry above the diagonal is $1$, $4$, $12$, which equals $n\cdot2^{n-1}$ for $n=1,2,3$. This suggests the formula

$$
A^n=
\begin{pmatrix}
2^n & n\cdot2^{n-1} \\
0 & 2^n \\
\end{pmatrix}.
$$

**Justification of the pattern**

Write $A=2I+N$, where

$$
N=
\begin{pmatrix}
0 & 1 \\
0 & 0 \\
\end{pmatrix}.
$$

Direct multiplication gives $N^2=0$. Since $2I$ commutes with $N$, the binomial theorem applies and all terms containing $N^2$ or higher powers vanish. Hence

$$
A^n=(2I+N)^n=2^nI+n\cdot2^{n-1}N,
$$

which agrees with the formula above. Assuming the formula for $n$, multiplication by $A$ gives the diagonal entry $2\cdot2^n=2^{n+1}$ and the upper-right entry $2^n+2\cdot n\cdot2^{n-1}=(n+1)2^n$, so the formula also holds for $n+1$.