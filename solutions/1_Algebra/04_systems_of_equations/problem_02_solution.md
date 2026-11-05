# Exercise 2. Gaussian Elimination — One Solution

## Question

Solve using Gaussian elimination:

$$
\begin{cases}
x+y+z=6, \\
2x-y+z=3, \\
x+2y-z=2.
\end{cases}
$$

After solving, substitute the result into all equations and check consistency.

## Solution

Start with the augmented matrix:

$$
\left[\begin{array}{ccc|c}
1&1&1&6\\2&-1&1&3\\1&2&-1&2
\end{array}\right].
$$

Apply $R_2\leftarrow R_2-2R_1$ and $R_3\leftarrow R_3-R_1$:

$$
\left[\begin{array}{ccc|c}
1&1&1&6\\0&-3&-1&-9\\0&1&-2&-4
\end{array}\right].
$$

Swap $R_2$ and $R_3$, then apply $R_3\leftarrow R_3+3R_2$:

$$
\left[\begin{array}{ccc|c}
1&1&1&6\\0&1&-2&-4\\0&0&-7&-21
\end{array}\right].
$$

Back substitution gives $z=3$, $y=-4+2z=2$, and $x=6-y-z=1$. There is a pivot in every variable column, so the solution is unique:

$$
\boxed{(x,y,z)=(1,2,3)}.
$$

**Check in all three original equations:**

$$
\begin{aligned}
1+2+3&=6,\\
2(1)-2+3&=3,\\
1+2(2)-3&=2.
\end{aligned}
$$
