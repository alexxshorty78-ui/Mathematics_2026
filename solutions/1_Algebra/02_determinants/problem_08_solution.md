# Exercise 8. Determinant of a Product

## Question

Let $A$ and $B$ be square matrices such that $\det A=3$ and $\det B=-5$. Compute $\det(AB)$, $\det(BA)$, and, if it exists, $\det(A^{-1}B)$. Explain why the first two results are equal even though usually $AB\neq BA$.

## Solution

The products in the question require $A$ and $B$ to have the same size. For square matrices of the same size, $\det(XY)=\det X\det Y$.

Thus,

$$
\det(AB)=\det A\det B=3(-5)=-15.
$$

Similarly,

$$
\det(BA)=\det B\det A=(-5)3=-15.
$$

Since $\det A=3\neq0$, the matrix $A$ is invertible and $\det(A^{-1})=1/\det A=1/3$. Therefore,

$$
\det(A^{-1}B)=\det(A^{-1})\det B=\frac{1}{3}(-5)=-\frac{5}{3}.
$$

The determinants of $AB$ and $BA$ are equal because both are the product $\det A\det B$, and multiplication of numbers is commutative. This does not imply that the matrices $AB$ and $BA$ themselves are equal.