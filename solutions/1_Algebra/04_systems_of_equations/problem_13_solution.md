# Exercise 13. Does Every Equation Add New Information?

## Question

Consider the system

$$
x_1+x_2=10,\qquad x_2+x_3=8,\qquad x_1-x_3=2.
$$

Solve it and check whether all three equations are independently necessary to describe the solution set. If one follows from the others, show this by calculation.

## Solution

Subtract the second equation from the first:

$$
(x_1+x_2)-(x_2+x_3)=10-8
\quad\Longrightarrow\quad
x_1-x_3=2.
$$

The third equation therefore follows from the first two and adds no constraint. With $x_2=s$ free, the first equation gives $x_1=10-s$ and the second gives $x_3=8-s$. Hence the full solution set is

$$
(x_1,x_2,x_3)=(10-s,s,8-s),\qquad s\in\mathbb{R}.
$$

For every $s$, the third left-hand side equals $(10-s)-(8-s)=2$.
