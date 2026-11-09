# Exercise 12. Homogeneous System

## Question

Solve

$$
\begin{cases}
x+2y-z=0, \\
2x+4y-2z=0, \\
x-y+2z=0. \\
\end{cases}
$$

Give all solutions in parametric form and explain why $(0,0,0)$ always satisfies a homogeneous system.

## Solution

The second equation is twice the first. Subtracting the first equation from the third gives

$$
-3y+3z=0.
$$

Thus $y=z$. The first equation then gives $x=-z$. With $z=s$ free, all solutions are

$$
(x,y,z)=(-s,s,s),\qquad s\in\mathbb{R}.
$$

Substitution gives $-s+2s-s=0$, $-2s+4s-2s=0$, and $-s-s+2s=0$. In any homogeneous linear system the right-hand side is zero, and setting all unknowns to zero makes each linear expression zero.
