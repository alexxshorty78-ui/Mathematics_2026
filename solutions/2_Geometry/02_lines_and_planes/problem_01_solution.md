# Exercise 1. Line Through Two Points

## Question

Find the equation of the line through $A=(1,2)$ and $B=(4,-1)$ in parametric and general form. Identify a direction vector and an example of a normal vector. Check that both points satisfy the equation you obtain.

## Solution

A direction vector is the difference of the two points:

$$
\overrightarrow{AB}=(4-1,-1-2)=(3,-3)=3(1,-1).
$$

Thus $v=(1,-1)$ is a direction vector. Using $A$ as the initial point gives the parametric equation

$$
(x,y)=(1,2)+t(1,-1),\qquad t\in\mathbb{R}.
$$

Equivalently,

$$
\begin{cases}
x=1+t, \\
y=2-t. \\
\end{cases}
$$

The vector $n=(1,1)$ is normal to the line because $n\cdot v=1-1=0$. The point-normal equation is

$$
(1,1)\cdot(x-1,y-2)=0.
$$

Therefore the general equation is

$$
x+y-3=0.
$$

For $A$, $1+2-3=0$; for $B$, $4-1-3=0$. In the parametric equation, $t=0$ gives $A$ and $t=3$ gives $B$. Both forms therefore describe the required line.
