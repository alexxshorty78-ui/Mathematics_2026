# Exercise 8. Intersection Point of a Line and a Plane

## Question

Find the intersection point of

$$
(x,y,z)=(1,0,2)+t(1,2,-1)
$$

with the plane $x+y+z=4$. Check the result by substituting it into both descriptions.

## Solution

The coordinate equations of the line are

$$
x=1+t,\qquad y=2t,\qquad z=2-t.
$$

Substitution into the plane equation gives

$$
(1+t)+2t+(2-t)=4,
\qquad 3+2t=4,
\qquad t=\frac12.
$$

The coefficient of $t$ is nonzero, so this is the only intersection parameter. The intersection point is

$$
H=\left(1+\frac12,2\cdot\frac12,2-\frac12\right)
=\left(\frac32,1,\frac32\right).
$$

**Check on the line:** the displacement from its base point is

$$
H-(1,0,2)=\left(\frac12,1,-\frac12\right)=\frac12(1,2,-1).
$$

Thus $H$ is on the line at $t=1/2$.

**Check on the plane:**

$$
\frac32+1+\frac32=4.
$$

Therefore, the unique intersection point is $H=(3/2,1,3/2)$.
