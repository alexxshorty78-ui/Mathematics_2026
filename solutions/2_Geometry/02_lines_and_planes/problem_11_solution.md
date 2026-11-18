# Exercise 11. Plane Containing a Line and a Point

## Question

Find the equation of the plane containing

$$
(x,y,z)=(1,0,2)+t(1,1,-1)
$$

and the point $P=(0,2,1)$. Check that both the entire line and the point lie in the plane you obtain.

## Solution

A point on the line is $A=(1,0,2)$, and its direction vector is $v=(1,1,-1)$. A second direction in the required plane is

$$
w=P-A=(0,2,1)-(1,0,2)=(-1,2,-1).
$$

The cross product gives a normal vector:

$$
\begin{aligned}
n=v\times w
&=\bigl(1(-1)-(-1)2,\;(-1)(-1)-1(-1),\;1\cdot2-1(-1)\bigr) \\
&=(1,2,3).
\end{aligned}
$$

Since $n\ne0$, the two directions are linearly independent and determine a unique plane through $A$. Its point-normal equation is

$$
(1,2,3)\cdot(x-1,y,z-2)=0.
$$

Therefore the required plane is

$$
x+2y+3z=7.
$$

For an arbitrary point $(1+t,t,2-t)$ on the line,

$$
(1+t)+2t+3(2-t)=1+t+2t+6-3t=7.
$$

Thus the entire line lies in the plane. Substituting $P=(0,2,1)$ also gives

$$
0+2\cdot2+3\cdot1=7.
$$

Both required containment conditions hold.
