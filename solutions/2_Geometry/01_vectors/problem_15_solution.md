# Exercise 15. Comparing Directions Using the Cosine of the Angle

## Question

Given

$$
a=(1,2,1),\qquad b=(2,4,2),\qquad c=(2,0,3).
$$

For each pair, compute

$$
\frac{u\cdot v}{\|u\|\,\|v\|}.
$$

Order the pairs by increasing angle between the vectors. Explain why for $a$ and $b$ the value is $1$ even though the vectors have different lengths.

## Solution

For the first pair, $b=2a$, and

$$
\frac{a\cdot b}{\|a\|\|b\|}=\frac{12}{\sqrt6\sqrt{24}}=1.
$$

This value is one because multiplying by a positive scalar changes length but not direction, so the angle between $a$ and $b$ is zero.

For the pair $a,c$,

$$
\frac{a\cdot c}{\|a\|\|c\|}=\frac{5}{\sqrt6\sqrt{13}}=\frac5{\sqrt{78}}.
$$

For the remaining pair,

$$
\frac{b\cdot c}{\|b\|\|c\|}=\frac{10}{\sqrt{24}\sqrt{13}}=\frac5{\sqrt{78}}.
$$

Cosine is strictly decreasing on $[0,\pi]$. Therefore, writing $\theta_{u,v}$ for the angle between $u$ and $v$, the order is

$$
\theta_{a,b}<\theta_{a,c}=\theta_{b,c}.
$$
