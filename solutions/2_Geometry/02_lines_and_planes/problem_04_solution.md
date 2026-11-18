# Exercise 4. Plane Through Three Points

## Question

Find the equation of the plane through

$$
A=(1,0,0),\quad B=(0,1,0),\quad C=(0,0,1).
$$

First construct two vectors lying in the plane, and then use the cross product. Check the resulting equation on all three points.

## Solution

Two vectors lying in the required plane are

$$
u=B-A=(-1,1,0),\qquad v=C-A=(-1,0,1).
$$

Their cross product is

$$
\begin{aligned}
u\times v
&=(1\cdot1-0\cdot0,\;0\cdot(-1)-(-1)\cdot1,\;(-1)\cdot0-1\cdot(-1)) \\
&=(1,1,1).
\end{aligned}
$$

This vector is nonzero, so the three points are not collinear and determine a unique plane. Taking $n=(1,1,1)$ as its normal and using $A$ gives

$$
(1,1,1)\cdot(x-1,y,z)=0.
$$

Therefore

$$
x+y+z=1.
$$

Substitution verifies all three points: $A$ gives $1+0+0=1$, $B$ gives $0+1+0=1$, and $C$ gives $0+0+1=1$.
