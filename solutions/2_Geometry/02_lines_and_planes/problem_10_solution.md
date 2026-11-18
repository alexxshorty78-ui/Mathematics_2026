# Exercise 10. Projection of a Point onto a Plane

## Question

Find the orthogonal projection of $P=(2,1,3)$ onto the plane $x+y+z=3$, and then find the reflection of $P$ across this plane. Check that the midpoint of the segment joining the point and its reflection lies on the plane.

## Solution

The plane has normal vector $n=(1,1,1)$ and equation $n\cdot X=3$. The perpendicular line through $P$ has the form

$$
X=P-\lambda n=(2-\lambda,1-\lambda,3-\lambda).
$$

Its intersection with the plane satisfies

$$
(2-\lambda)+(1-\lambda)+(3-\lambda)=3,
\qquad 6-3\lambda=3,
\qquad \lambda=1.
$$

Therefore, the orthogonal projection is

$$
H=P-n=(1,0,2).
$$

This point lies on the plane, since $1+0+2=3$. Moreover,

$$
P-H=(1,1,1)=n,
$$

so the joining segment is perpendicular to the plane, as required for an orthogonal projection.

The reflection $P'$ lies the same distance from the plane on the opposite side, with $H$ as the midpoint. Hence

$$
P'=2H-P=2(1,0,2)-(2,1,3)=(0,-1,1).
$$

The midpoint check gives

$$
\frac{P+P'}2
=\left(\frac{2+0}{2},\frac{1-1}{2},\frac{3+1}{2}\right)
=(1,0,2)=H.
$$

Its coordinate sum is $1+0+2=3$, so it lies on the plane. Also $P-H=n$ and $P'-H=-n$, confirming equal distances on opposite sides.

**Projection:** $H=(1,0,2)$. **Reflection:** $P'=(0,-1,1)$.
