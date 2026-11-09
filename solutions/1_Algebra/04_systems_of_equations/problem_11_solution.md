# Exercise 11. A Parameter in a System of Three Equations

## Question

Analyze the number of solutions depending on $t$:

$$
\begin{cases}
x+y+z=1, \\
x+ty+z=2, \\
x+y+tz=3. \\
\end{cases}
$$

Use elimination and separately analyze the parameter values for which a standard calculation step ceases to be valid.

## Solution

Subtract the first equation from the second and third. The reduced system is equivalent to the original for every $t$.

$$
\begin{cases}
x+y+z=1, \\
(t-1)y=1, \\
(t-1)z=2. \\
\end{cases}
$$

If $t\ne 1$, the last two equations determine $y$ and $z$. Substituting them into the first equation gives the unique solution

$$
(x,y,z)=\left(1-\frac{3}{t-1},\frac{1}{t-1},\frac{2}{t-1}\right).
$$

If $t=1$, division by $t-1$ is undefined. The second reduced equation becomes $0=1$, so the system has no solution. These cases exhaust all values of $t$.
