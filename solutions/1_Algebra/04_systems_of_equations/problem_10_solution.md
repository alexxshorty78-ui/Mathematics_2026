# Exercise 10. A Polynomial Through Three Points

## Question

Find a polynomial $p(x)=ax^2+bx+c$ whose graph passes through $(0,1)$, $(1,3)$, and $(2,9)$. Reduce the problem to a system of equations and check the result by substituting all three points.

## Solution

Substitute each point into $p(x)=ax^2+bx+c$:

$$
\begin{aligned}
p(0)=1&\quad\Longrightarrow\quad c=1,\\
p(1)=3&\quad\Longrightarrow\quad a+b+c=3,\\
p(2)=9&\quad\Longrightarrow\quad 4a+2b+c=9.
\end{aligned}
$$

Thus the coefficients satisfy the linear system

$$
\begin{cases}
c=1, \\
a+b+c=3, \\
4a+2b+c=9. \\
\end{cases}
$$

Using $c=1$, the last two equations become $a+b=2$ and $4a+2b=8$. Subtract twice $a+b=2$ from $4a+2b=8$:

$$
2a=4\quad\Longrightarrow\quad a=2.
$$

Then $b=2-a=0$. Therefore

$$
(a,b,c)=(2,0,1),
\qquad
p(x)=2x^2+1.
$$

These elimination steps determine all three coefficients uniquely.

**Check all three points:**

$$
\begin{aligned}
p(0)&=2(0)^2+1=1,\\
p(1)&=2(1)^2+1=3,\\
p(2)&=2(2)^2+1=9.
\end{aligned}
$$
