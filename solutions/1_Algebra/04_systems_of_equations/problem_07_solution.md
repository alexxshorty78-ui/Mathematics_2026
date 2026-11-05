# Exercise 7. Choosing a Method Deliberately

## Question

Do not solve all of the following systems completely. For each situation, choose the method that best uses its structure and justify your choice:

1. one system with a triangular coefficient matrix

$$
\begin{cases}
2x-y=3, \\
4y=8; \\
\end{cases}
$$

2. three systems $Ax=b_i$ with the same invertible matrix $A$, when $A^{-1}$ is already known;
3. one $3\times3$ system for which the inverse matrix is not given and the goal is only to find one solution vector.

For case 1, carry out the chosen method completely. For cases 2 and 3, describe the plan and indicate which part of the computation would be reusable or unnecessary. Do not judge a method by its name alone — refer to the number of right-hand sides and the structure of the matrix.

## Solution

### Case 1: A triangular system

Choose **back substitution**, because the second equation already contains only $y$:

$$
4y=8\quad\Longrightarrow\quad y=2.
$$

Substitute into the first equation:

$$
2x-2=3
\quad\Longrightarrow\quad
x=\frac52.
$$

Thus

$$
(x,y)=\left(\frac52,2\right).
$$

The check is $2(5/2)-2=3$ and $4(2)=8$. No elimination or inverse calculation is necessary because the system is already triangular.

### Case 2: Three right-hand sides and a known inverse

Since the same invertible matrix $A$ is used and $A^{-1}$ is already available, compute

$$
\mathbf{x}_i=A^{-1}\mathbf{b}_i,\qquad i=1,2,3.
$$

The same inverse is reused for all three right-hand sides. Equivalently, multiply once by the matrix containing all three columns:

$$
\begin{pmatrix}
\mathbf{x}_1 & \mathbf{x}_2 & \mathbf{x}_3 \\
\end{pmatrix} =
A^{-1}
\begin{pmatrix}
\mathbf{b}_1 & \mathbf{b}_2 & \mathbf{b}_3 \\
\end{pmatrix}.
$$

There is no need to recompute the inverse or perform a separate elimination from the beginning for each system.

### Case 3: One system and no known inverse

Choose **Gaussian elimination** on $[A\mid\mathbf{b}]$. Reduce to row echelon form and use back substitution if there is a unique solution. If a zero row or a contradiction appears, identify free variables or conclude that no solution exists.

Only one right-hand side is given, so calculating the entire inverse would introduce unnecessary work. If more right-hand sides with the same $A$ were later supplied, the elimination operations (or an LU factorization, when applicable) could be reused. No numerical solution can be computed here because the entries of this system are not specified.
