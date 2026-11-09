### Exercise 13. A Recurrence Written in Matrix Form
Let

$$
F=
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}.
$$

Compute $F^2$, $F^3$, $F^4$, and $F^5$. Compare the numbers obtained with the sequence

$$
0,1,1,2,3,5,8,\ldots
$$

and describe the relationship you observe. Then compute

$$
F
\begin{pmatrix}
a \\
b \\
\end{pmatrix}
$$

and explain how this multiplication performs one recurrence step: it creates the sum of two consecutive terms and keeps one of them for the next step.

> **Why this exercise:** shows the connection between matrix powers and a simple numerical recurrence.

#### Solution

Successive multiplication by $F$ gives

$$
F^2=
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix},
\qquad F^3=
\begin{pmatrix}
3 & 2 \\
2 & 1 \\
\end{pmatrix},
$$

$$
F^4=
\begin{pmatrix}
5 & 3 \\
3 & 2 \\
\end{pmatrix},
\qquad F^5=
\begin{pmatrix}
8 & 5 \\
5 & 3 \\
\end{pmatrix}.
$$

Let $f_0=0$, $f_1=1$, and $f_{n+1}=f_n+f_{n-1}$ for $n\ge 1$. The entries in $F^n$ are consecutive Fibonacci numbers. The top-left entry is $f_{n+1}$, both off-diagonal entries are $f_n$, and the bottom-right entry is $f_{n-1}$.

Multiplying an arbitrary vector by $F$ gives

$$
F
\begin{pmatrix}
a \\
b \\
\end{pmatrix}=
\begin{pmatrix}
a+b \\
a \\
\end{pmatrix}.
$$

For input $(a,b)=(f_n,f_{n-1})$, this produces $(f_{n+1},f_n)$. The first coordinate is the next term, and the second retains the previous first coordinate for the next addition.

**Verification of the pattern.** The columns of $F$ are the pairs $(f_2,f_1)$ and $(f_1,f_0)$. Multiplication on the left by $F$ advances both pairs by one step. Thus the columns of $F^n$ are $(f_{n+1},f_n)$ and $(f_n,f_{n-1})$ for all $n\ge 1$.
