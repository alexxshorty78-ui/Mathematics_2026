# Exercise 5. Relative Position of Two Lines

## Question

Analyze the position of

$$
L_1:(x,y,z)=(1,1,0)+t(1,2,1),
$$

$$
L_2:(x,y,z)=(2,0,1)+s(0,1,-1).
$$

If they intersect, give the intersection point. If not, determine whether they are parallel or skew. Justify the classification.

## Solution

The direction vectors are $v_1=(1,2,1)$ and $v_2=(0,1,-1)$. They are not scalar multiples: any multiple of $v_2$ has first coordinate zero, whereas $v_1$ has first coordinate one. Thus the lines are not parallel.

An intersection would require a common pair of parameters satisfying

$$
\begin{cases}
1+t=2, \\
1+2t=s, \\
t=1-s. \\
\end{cases}
$$

The first equation gives $t=1$. The second then requires $s=3$, but the third requires $s=0$. These conditions are inconsistent, so the lines have no intersection point.

Since the lines are neither parallel nor intersecting, they are **skew**.

As an independent check, the displacement between their initial points is $w=(2,0,1)-(1,1,0)=(1,-1,1)$, and

$$
v_1\times v_2=(-3,1,1),\qquad w\cdot(v_1\times v_2)=-3-1+1=-3\ne0.
$$

The nonzero scalar triple product confirms that the two lines are not coplanar.
