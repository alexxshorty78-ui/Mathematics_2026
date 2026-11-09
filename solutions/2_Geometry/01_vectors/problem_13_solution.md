# Exercise 13. Do Four Points Lie in One Plane?

## Question

Given

$$
A=(0,0,0),\qquad B=(1,2,0),\qquad C=(0,1,1),\qquad D=(2,5,1).
$$

1. Construct $\overrightarrow{AB}$ and $\overrightarrow{AC}$.
2. Find $n=\overrightarrow{AB}\times\overrightarrow{AC}$.
3. Construct $\overrightarrow{AD}$ and check whether $\overrightarrow{AD}\cdot n=0$.
4. Based on this, decide whether $D$ lies in the plane determined by $A,B,C$, and justify the criterion.

## Solution

Two directions in the plane are

$$
\overrightarrow{AB}=(1,2,0),\qquad \overrightarrow{AC}=(0,1,1).
$$

Their cross product is

$$
n=\overrightarrow{AB}\times\overrightarrow{AC}=(2,-1,1).
$$

For $\overrightarrow{AD}=(2,5,1)$, the dot product is

$$
\overrightarrow{AD}\cdot n=2\cdot2+5(-1)+1\cdot1=4-5+1=0.
$$

The nonzero cross product $n$ is normal to the plane determined by $A,B,C$. The directions perpendicular to $n$ are exactly the directions in that plane. Since $\overrightarrow{AD}\cdot n=0$, the displacement from $A$ to $D$ has one of those directions, so $D$ lies in the plane.

As a direct check, $\overrightarrow{AD}=2\overrightarrow{AB}+\overrightarrow{AC}$, so the displacement is a linear combination of two directions in the plane.
