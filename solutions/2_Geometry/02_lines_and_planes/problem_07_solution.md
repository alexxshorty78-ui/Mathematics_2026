# Exercise 7. A Line Relative to a Plane

## Question

For

$$
L:(x,y,z)=(1,1,0)+t(1,-1,0),\qquad \Pi:x+y+z=2,
$$

determine whether the line intersects the plane at one point, is parallel to it, or lies in it. Explain the role of the dot product of the direction vector and the normal vector.

## Solution

The line has direction vector $v=(1,-1,0)$, and the plane has normal vector $n=(1,1,1)$. Their dot product is

$$
n\cdot v=1\cdot1+1\cdot(-1)+1\cdot0=0.
$$

Thus the line's direction is perpendicular to the normal and parallel to the plane. This condition alone allows either a line contained in the plane or a parallel line with no common points.

The base point $A=(1,1,0)$ satisfies

$$
1+1+0=2.
$$

Therefore, the base point lies in the plane. More generally, every point of the line has coordinates

$$
(x,y,z)=(1+t,1-t,0),\qquad t\in\mathbb R,
$$

and satisfies

$$
x+y+z=(1+t)+(1-t)+0=2.
$$

**The entire line lies in the plane**, so there are infinitely many common points. In general, a nonzero dot product $n\cdot v$ gives one intersection point. A zero dot product requires checking a point on the line to distinguish containment from parallelism with no common points.
