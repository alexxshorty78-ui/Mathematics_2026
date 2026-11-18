# Exercise 6. Angle Between Planes

## Question

Given

$$
\Pi_1:x+y+z=1,\qquad \Pi_2:x-y=2.
$$

First use the normal vectors to decide whether the planes are parallel. If not, compute the angle between them and explain why the normal vectors alone are enough for this calculation.

## Solution

The coefficients of the coordinates give normal vectors

$$
n_1=(1,1,1),\qquad n_2=(1,-1,0).
$$

These nonzero vectors are not scalar multiples: the third coordinate of every multiple of $n_2$ is zero, whereas the third coordinate of $n_1$ is one. Therefore, the planes are not parallel.

The angle $\theta$ between two planes is the smaller angle between their normal directions. Hence

$$
\cos\theta=\frac{|n_1\cdot n_2|}{\|n_1\|\,\|n_2\|},\qquad 0\le\theta\le\frac{\pi}{2}.
$$

Here

$$
n_1\cdot n_2=1\cdot1+1\cdot(-1)+1\cdot0=0,
\qquad \|n_1\|=\sqrt3,\qquad \|n_2\|=\sqrt2.
$$

It follows that

$$
\cos\theta=0,\qquad \theta=\frac{\pi}{2}=90^\circ.
$$

**The planes are perpendicular.** A normal vector determines a plane's orientation. The right-hand sides of the plane equations affect their positions, but not the angle between them, so the normal vectors alone determine this angle.
