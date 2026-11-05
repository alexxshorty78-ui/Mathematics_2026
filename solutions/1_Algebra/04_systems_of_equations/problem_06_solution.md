# Exercise 6. A System with a Parameter — Which Cases Actually Occur?

## Question

Analyze, depending on the parameter $a$, the system

$$
\begin{cases}
x+y=2, \\
ax+ay=4. \\
\end{cases}
$$

Among the three possibilities — exactly one solution, infinitely many solutions, no solution — determine which actually occur and for which values of $a$. If one type cannot occur, explain why.

## Solution

Treat $a$ as a real parameter. Eliminate the first entry of the second row:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
a & a & \mid & 4 \\
\end{pmatrix}
\xrightarrow{R_2\leftarrow R_2-aR_1}
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 4-2a \\
\end{pmatrix}.
$$

This operation is valid for every $a$; it does not involve division by $a$.

- If $a=2$, the second row is $0=0$. Only $x+y=2$ remains, so there are infinitely many solutions:
  $(x,y)=(2-t,t),\ t\in\mathbb{R}$.
- If $a\ne2$, the second row requires $0=4-2a\ne0$, a contradiction. There is no solution.

Exactly one solution cannot occur: the coefficient rows are always proportional, so there can never be two pivots for the two unknowns. When the system is consistent, one variable remains free.

For $a=2$, substitution confirms $(2-t)+t=2$ and $2(2-t)+2t=4$.
