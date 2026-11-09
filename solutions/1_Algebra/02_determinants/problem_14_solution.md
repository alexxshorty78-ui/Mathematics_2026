# Exercise 14. A System of Equations and the Determinant

## Question

Consider the system $Ax=b$, where

$$
A=
\begin{pmatrix}
1 & 2 \\
k & 4 \\
\end{pmatrix}.
$$

For which values of $k$ does the system have exactly one solution for every $b$? For the remaining value, give an example of a right-hand side $b$ for which the system has infinitely many solutions, and an example for which it has no solution.

## Solution

The determinant is $\det A=4-2k$. Thus $A$ is invertible for $k\neq 2$, and $x=A^{-1}b$ is the unique solution for every $b$.

At $k=2$ the second row of $A$ is twice the first row. For $x=(x_1,x_2)^T$ and $b=(b_1,b_2)^T$, the system is

$$
\begin{cases}
x_1+2x_2=b_1, \\
2x_1+4x_2=b_2. \\
\end{cases}
$$

**Infinitely many solutions**

$$
b=\begin{pmatrix}
3 \\
6 \\
\end{pmatrix}.
$$

The second equation is twice the first. All solutions are $(x_1,x_2)=(3-2s,s)$ with $s\in\mathbb{R}$.

**No solution**

$$
b=\begin{pmatrix}
3 \\
5 \\
\end{pmatrix}.
$$

The first equation implies $2x_1+4x_2=6$, whereas the second requires $2x_1+4x_2=5$.
