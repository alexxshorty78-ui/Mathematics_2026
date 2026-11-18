# Exercise 14. Contrast: Intersection and Parallelism

## Question

From the point $P=(0,0,1)$, two lines are drawn with direction vectors

$$
v_1=(2,1,-1),\qquad v_2=(2,1,0).
$$

For each line, analyze its position relative to the plane $z=0$.

For the line that intersects the plane, find the intersection point. For the other line, explain how you can recognize parallelism without solving an equation.

## Solution

The plane $\Pi:z=0$ has normal vector $n=(0,0,1)$.

### First line

The line with direction $v_1$ is

$$
L_1:(x,y,z)=(0,0,1)+t(2,1,-1)=(2t,t,1-t),\qquad t\in\mathbb{R}.
$$

Its direction satisfies

$$
n\cdot v_1=(0,0,1)\cdot(2,1,-1)=-1\ne0.
$$

Therefore it crosses the plane at exactly one point. The plane condition $z=0$ gives $1-t=0$, so $t=1$. The intersection point is

$$
L_1\cap\Pi=\{(2,1,0)\}.
$$

This point equals $(0,0,1)+1(2,1,-1)$ and has zero third coordinate, verifying membership in both the line and the plane.

### Second line

The line with direction $v_2$ is

$$
L_2:(x,y,z)=(0,0,1)+s(2,1,0)=(2s,s,1),\qquad s\in\mathbb{R}.
$$

Its direction satisfies

$$
n\cdot v_2=(0,0,1)\cdot(2,1,0)=0.
$$

Thus its direction is parallel to the plane: moving along the line does not change the $z$ coordinate. The starting point has $z=1$, so it is outside the plane. Consequently the entire line remains at $z=1$, and $L_2$ is parallel to the plane with no common points.
