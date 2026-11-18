# Exercise 13. Closest Point on a Plane

## Question

Find the point on the plane $x+2y+2z=4$ closest to $P=(3,0,0)$. Give the distance and check that the segment joining the two points is perpendicular to the plane.

## Solution

The plane has normal vector $n=(1,2,2)$. The closest point is the orthogonal projection of $P$ onto the plane, so it lies on the normal line through $P$. Write it as

$$
H=P+\lambda n=(3+\lambda,2\lambda,2\lambda).
$$

Substitution into the plane equation gives

$$
(3+\lambda)+2(2\lambda)+2(2\lambda)=4,
\qquad 3+9\lambda=4,
\qquad \lambda=\frac19.
$$

Therefore the closest point is

$$
H=\left(\frac{28}{9},\frac29,\frac29\right).
$$

It lies on the plane because

$$
\frac{28}{9}+2\cdot\frac29+2\cdot\frac29
=\frac{36}{9}=4.
$$

The joining vector is

$$
H-P=\left(\frac19,\frac29,\frac29\right)=\frac19n.
$$

It is a nonzero scalar multiple of the plane's normal vector, so the segment $PH$ is perpendicular to the plane. Its length is

$$
\|H-P\|=\sqrt{\frac{1+4+4}{81}}=\frac13.
$$

The point-to-plane distance formula confirms the same value:

$$
\frac{|3+2\cdot0+2\cdot0-4|}{\sqrt{1^2+2^2+2^2}}=\frac13.
$$

For any other point $Q$ on the plane, $Q-H$ lies in the plane and is perpendicular to $P-H$. Thus

$$
\|P-Q\|^2=\|P-H\|^2+\|Q-H\|^2\ge\|P-H\|^2.
$$

Equality holds only when $Q=H$, which also verifies that $H$ is the unique closest point.
