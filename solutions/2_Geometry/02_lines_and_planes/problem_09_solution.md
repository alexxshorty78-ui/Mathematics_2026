# Exercise 9. Distances

## Question

Compute:

1. the distance from $P=(2,3)$ to the line $3x+4y-10=0$,
2. the distance from $Q=(2,-1,3)$ to the plane $2x-2y+z-4=0$.

Compare the two formulas and explain their common connection with the normal direction.

## Solution

### 1. Distance from the point to the line

The distance from $(x_0,y_0)$ to $ax+by+c=0$ is

$$
\delta=\frac{|ax_0+by_0+c|}{\sqrt{a^2+b^2}}.
$$

For $P=(2,3)$ and the normal vector $(3,4)$,

$$
\delta_1=\frac{|3\cdot2+4\cdot3-10|}{\sqrt{3^2+4^2}}
=\frac{|6+12-10|}{5}=\frac85.
$$

As a check, the perpendicular foot on the line is

$$
H_1=(2,3)-\frac{8}{25}(3,4)
=\left(\frac{26}{25},\frac{43}{25}\right).
$$

It lies on the line because

$$
3\cdot\frac{26}{25}+4\cdot\frac{43}{25}-10
=\frac{78+172-250}{25}=0.
$$

The displacement $P-H_1=(8/25)(3,4)$ is normal to the line and has length $(8/25)\cdot5=8/5$.

### 2. Distance from the point to the plane

The distance from $(x_0,y_0,z_0)$ to $ax+by+cz+d=0$ is

$$
\delta=\frac{|ax_0+by_0+cz_0+d|}{\sqrt{a^2+b^2+c^2}}.
$$

For $Q=(2,-1,3)$ and the normal vector $(2,-2,1)$,

$$
\delta_2=\frac{|2\cdot2-2\cdot(-1)+3-4|}{\sqrt{2^2+(-2)^2+1^2}}
=\frac{|4+2+3-4|}{3}=\frac53.
$$

The perpendicular foot is

$$
H_2=(2,-1,3)-\frac59(2,-2,1)
=\left(\frac89,\frac19,\frac{22}{9}\right).
$$

It lies on the plane because

$$
2\cdot\frac89-2\cdot\frac19+\frac{22}{9}-4
=\frac{16-2+22-36}{9}=0.
$$

The displacement $Q-H_2=(5/9)(2,-2,1)$ is normal to the plane and has length $(5/9)\cdot3=5/3$.

### Common geometric formula

For either a line in the plane or a plane in space, write the equation as $n\cdot X=k$, with $n\ne0$. For a given point $X_0$, the distance and perpendicular foot are

$$
\delta=\frac{|n\cdot X_0-k|}{\|n\|},
\qquad H=X_0-\frac{n\cdot X_0-k}{\|n\|^2}n.
$$

Both formulas measure the component of displacement along the unit normal. The shortest segment from a point to the line or plane follows that normal direction; the absolute value makes its length nonnegative.
