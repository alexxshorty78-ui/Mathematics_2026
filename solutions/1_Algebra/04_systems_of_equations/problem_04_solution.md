# Exercise 4. Infinitely Many Solutions

## Question

Solve

$$
\begin{cases}
x+y+z=2, \\
2x+2y+2z=4, \\
x-y+z=0.
\end{cases}
$$

Give the solution in parametric form, identify a free variable, and for one chosen parameter value check that the resulting point really satisfies the system.

## Solution

Use Gaussian elimination:

$$
\left[\begin{array}{ccc|c}
1&1&1&2\\2&2&2&4\\1&-1&1&0
\end{array}\right].
$$

Apply $R_2\leftarrow R_2-2R_1$ and $R_3\leftarrow R_3-R_1$, then swap $R_2$ and $R_3$:

$$
\left[\begin{array}{ccc|c}
1&1&1&2\\0&-2&0&-2\\0&0&0&0
\end{array}\right].
$$

The second row gives $y=1$. The first then gives $x+z=1$. There are two pivots and three unknowns, so $z$ is a free variable. Set $z=t$, where $t\in\mathbb{R}$. All solutions are

$$
\boxed{(x,y,z)=(1-t,1,t),\qquad t\in\mathbb{R}}.
$$

There are infinitely many solutions. Indeed, for every real $t$,

$$
\begin{aligned}
(1-t)+1+t&=2,\\
2(1-t)+2+2t&=4,\\
(1-t)-1+t&=0.
\end{aligned}
$$

For example, choosing $t=0$ gives $(1,1,0)$, which satisfies the three equations: $1+1+0=2$, $2+2+0=4$, and $1-1+0=0$.
