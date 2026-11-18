# Exercise 12. Intersection Line of Two Planes

## Question

Find a parametric equation of the line that is the intersection of

$$
x+y+z=3,\qquad x-y+z=1.
$$

Find its direction vector in two ways: from the system of equations and from the cross product of the normal vectors. Compare the results.

## Solution

Subtracting the second plane equation from the first gives

$$
2y=2,\qquad y=1.
$$

Substituting $y=1$ into either original equation gives $x+z=2$. Set $z=-t$, where $t\in\mathbb{R}$. Then $x=2+t$, so the intersection line is

$$
L:(x,y,z)=(2,1,0)+t(1,0,-1),\qquad t\in\mathbb{R}.
$$

The system therefore gives the direction vector

$$
v=(1,0,-1).
$$

The normal vectors of the two planes are $n_1=(1,1,1)$ and $n_2=(1,-1,1)$. Their cross product is

$$
\begin{aligned}
n_1\times n_2
&=\bigl(1\cdot1-1(-1),\;1\cdot1-1\cdot1,\;1(-1)-1\cdot1\bigr) \\
&=(2,0,-2)=2v.
\end{aligned}
$$

This nonzero cross product is perpendicular to both normals, so it is parallel to both planes. It is a nonzero scalar multiple of $v$, and the two methods give the same line direction.

For every $t\in\mathbb{R}$, substitution into the original equations gives

$$
\begin{aligned}
(2+t)+1-t&=3, \\
(2+t)-1-t&=1.
\end{aligned}
$$

Conversely, every common point satisfies $y=1$ and $x+z=2$, and hence has this parametric form. The line describes the complete intersection.
