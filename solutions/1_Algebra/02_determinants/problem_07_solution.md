# Exercise 7. Using Properties Instead of Recomputing

## Question

Suppose that for a $3\times3$ matrix, $\det A=-4$. Compute

$$
\det(2A),\qquad \det(A^T),\qquad \det(A^2),\qquad \det(-A).
$$

Justify each answer using the appropriate property.

## Solution

For a scalar multiple of a $3\times3$ matrix, $\det(cA)=c^3\det A$. Hence,

$$
\det(2A)=2^3(-4)=-32.
$$

The determinant of a transpose is unchanged:

$$
\det(A^T)=\det A=-4.
$$

The determinant of a product is the product of the determinants:

$$
\det(A^2)=\det(A)\det(A)=(-4)^2=16.
$$

Since $-A=(-1)A$,

$$
\det(-A)=(-1)^3\det A=-1(-4)=4.
$$