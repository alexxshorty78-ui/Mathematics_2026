### Exercise 12. Formula for a Matrix Power
Let

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}.
$$

Compute $A^2$, $A^3$, and $A^4$, and use them to formulate a conjecture for $A^n$. Then do not stop after checking one more case: assume the formula is true for $n$, multiply by $A$, and explain why you obtain exactly the formula for $n+1$.

> **Why this exercise:** teaches how to recognize a pattern and formulate a generalization from several computations.

#### Solution

Successive multiplication on the right by $A$ gives

$$
A^2=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},
\qquad A^3=
\begin{pmatrix}
1 & 3 \\
0 & 1 \\
\end{pmatrix},
\qquad A^4=
\begin{pmatrix}
1 & 4 \\
0 & 1 \\
\end{pmatrix}.
$$

These powers suggest that for every integer $n\ge 1$,

$$
A^n=
\begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix}.
$$

**Proof by induction.** The formula gives $A$ when $n=1$. If it holds for some $n\ge 1$, then

$$
A^{n+1}=A^n A=
\begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 1+n \\
0 & 1 \\
\end{pmatrix}.
$$

The upper-right entry increases by $1$ and the other entries retain their values. This is the proposed formula with $n+1$ in place of $n$, completing the induction. It also holds at $n=0$, when $A^0=I_2$.
