# Exercise 3. Inconsistent System

## Question

Solve or show that the system is inconsistent:

$$
\begin{cases}
x+2y=3, \\
2x+4y=7.
\end{cases}
$$

Show how the contradiction appears in the matrix after elimination and interpret it in terms of equations.

## Solution

The augmented matrix is

$$
\left[\begin{array}{cc|c}
1&2&3\\2&4&7
\end{array}\right].
$$

Apply $R_2\leftarrow R_2-2R_1$:

$$
\left[\begin{array}{cc|c}
1&2&3\\0&0&1
\end{array}\right].
$$

The second row represents $0x+0y=1$, or $0=1$. This is a contradiction. Equivalently, twice the first original equation would require $2x+4y=6$, whereas the second requires $2x+4y=7$.

Therefore the system is inconsistent and its solution set is

$$
\boxed{\varnothing}.
$$
