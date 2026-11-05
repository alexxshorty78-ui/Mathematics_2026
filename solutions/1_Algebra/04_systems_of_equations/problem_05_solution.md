# Exercise 5. Row Echelon Form and Number of Solutions

## Question

For the augmented matrix

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 3 \\
0 & 1 & 2 & \mid & 1 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

determine the number of solutions and write them in parametric form. Explain how you know how many variables may be chosen freely.

## Solution

The matrix represents

$$
\begin{cases}
x+2y-z=3, \\
y+2z=1, \\
0=0. \\
\end{cases}
$$

There are pivots in the $x$ and $y$ columns, but no pivot in the $z$ column. The zero row gives no restriction and there is no contradiction. Thus there is one free variable: three unknowns minus two pivots.

Set $z=t$, where $t\in\mathbb{R}$. Back substitution gives

$$
y=1-2t,
\qquad
x=3-2y+z=3-2(1-2t)+t=1+5t.
$$

Therefore there are infinitely many solutions:

$$
(x,y,z)=(1+5t,1-2t,t),\qquad t\in\mathbb{R}.
$$

**Check:**

$$
\begin{aligned}
(1+5t)+2(1-2t)-t&=3,\\
(1-2t)+2t&=1.
\end{aligned}
$$
