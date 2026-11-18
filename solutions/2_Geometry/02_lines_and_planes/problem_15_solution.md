# Exercise 15. Complete Classification of a Line Relative to a Plane

## Question

Let

$$
L:p+tv,\qquad \Pi:n\cdot x=d.
$$

State the conditions distinguishing the three cases: one intersection point, parallel with no common points, and the line contained in the plane. Then illustrate each case with your own simple numerical example.

## Solution

Assume $p,v,n\in\mathbb{R}^3$, $d\in\mathbb{R}$, $v\ne0$, and $n\ne0$, so that $L$ is a line and $\Pi$ is a plane. A point on $L$ has the form $x=p+tv$, where $t\in\mathbb{R}$. It lies on $\Pi$ precisely when

$$
n\cdot(p+tv)=d,
\qquad t(n\cdot v)=d-n\cdot p.
$$

This scalar equation yields all three cases.

### One intersection point

If $n\cdot v\ne0$, there is exactly one parameter value

$$
t_0=\frac{d-n\cdot p}{n\cdot v}.
$$

The unique intersection point is

$$
x_0=p+\frac{d-n\cdot p}{n\cdot v}\,v.
$$

For example, take

$$
\Pi:z=0,\qquad L:(x,y,z)=(0,0,1)+t(0,0,-1).
$$

Here $n=(0,0,1)$, $d=0$, and $n\cdot v=-1$. The equation $1-t=0$ gives $t=1$, and the intersection point is $(0,0,0)$.

### Parallel with no common points

If $n\cdot v=0$ and $n\cdot p\ne d$, the parameter equation has no solution. The direction vector is parallel to the plane, but the starting point lies outside it. Hence the line has no point in common with the plane.

For example, take

$$
\Pi:z=0,\qquad L:(x,y,z)=(0,0,1)+t(1,0,0).
$$

Here $n\cdot v=0$ and $n\cdot p=1\ne0=d$. Every point on the line has $z=1$, so no point lies on the plane.

### Line contained in the plane

If $n\cdot v=0$ and $n\cdot p=d$, the parameter equation is satisfied for every $t\in\mathbb{R}$. The starting point lies in the plane, and the direction remains within it. Thus the whole line lies in the plane, giving infinitely many common points.

For example, take

$$
\Pi:z=0,\qquad L:(x,y,z)=(1,0,0)+t(0,1,0).
$$

Here $n\cdot v=0$ and $n\cdot p=0=d$. Every point on the line is $(1,t,0)$ and therefore satisfies the plane equation.

The condition $n\cdot v=0$ alone distinguishes a direction parallel to the plane. The additional check $n\cdot p=d$ determines whether the line is contained in the plane or disjoint from it.
