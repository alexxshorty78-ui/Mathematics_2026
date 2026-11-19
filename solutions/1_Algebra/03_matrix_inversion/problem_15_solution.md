# Exercise 15 – Two Methods for Solving the Same System

## Question

For

$$
A=
\begin{pmatrix}
2&1 \\
1&3 \\
\end{pmatrix},
\qquad
b=
\begin{pmatrix}
7 \\
8 \\
\end{pmatrix}
$$

solve $Ax=b$ in two ways:

1. Using $A^{-1}b$.
2. Using Gaussian elimination.

Compare both solutions, the number of essential steps, and state which method was simpler in this example.

## Solution

### 1. Method 1: Using the Inverse Matrix

We start with:

$$
Ax=b
$$

Multiplying both sides by $A^{-1}$ gives:

$$
x=A^{-1}b
$$

First, calculate the determinant of A:

$$
\det(A)=(2)(3)-(1)(1)=5
$$

Since the determinant is not zero, the inverse exists.

Calculate the inverse:

$$
A^{-1}
= \frac{1}{5}
\begin{pmatrix}
3&-1 \\
-1&2 \\
\end{pmatrix}
$$

Now calculate $x=A^{-1}b$:

$$
x=
\frac{1}{5}
\begin{pmatrix}
3&-1 \\
-1&2 \\
\end{pmatrix}
\begin{pmatrix}
7 \\
8 \\
\end{pmatrix}
$$

$$
x=
\frac{1}{5}
\begin{pmatrix}
21-8 \\
-7+16 \\
\end{pmatrix}
$$

Therefore:

$$
x=
\begin{pmatrix}
\frac{13}{5} \\
\frac{9}{5} \\
\end{pmatrix}
$$

### 2. Method 2: Using Gaussian Elimination

Start with the augmented matrix.

$$
\begin{pmatrix}
2 & 1 & \mid & 7 \\
1 & 3 & \mid & 8 \\
\end{pmatrix}
$$

Apply $R_2\leftarrow R_2-\frac12R_1$ to eliminate the first entry in the second row.

$$
\begin{pmatrix}
2 & 1 & \mid & 7 \\
0 & \frac52 & \mid & \frac92 \\
\end{pmatrix}
$$

The second equation gives $x_2=(\frac92)/(\frac52)=\frac95$. Substituting into the first equation gives $x_1=(7-\frac95)/2=\frac{13}{5}$. Thus

$$
x=
\begin{pmatrix}
\frac{13}{5} \\
\frac95 \\
\end{pmatrix}.
$$

### 3. Verify the Solution

Both methods give the same solution:

$$
x=
\begin{pmatrix}
\frac{13}{5} \\
\frac95 \\
\end{pmatrix}
$$

Substitute it into the original equation:

$$
Ax=
\begin{pmatrix}
2&1 \\
1&3 \\
\end{pmatrix}
\begin{pmatrix}
\frac{13}{5} \\
\frac95 \\
\end{pmatrix}
$$

$$
= \begin{pmatrix}
\frac{26}{5}+\frac95 \\
\frac{13}{5}+\frac{27}{5} \\
\end{pmatrix}
= \begin{pmatrix}
7 \\
8 \\
\end{pmatrix}
=b
$$

The solution is correct.

### 4. Compare the Methods

Both methods give $x_1=\frac{13}{5}$ and $x_2=\frac95$.

- The inverse method has three main steps. Compute the determinant, form $A^{-1}$, and multiply $A^{-1}b$.
- Gaussian elimination also has three main steps. Eliminate the entry below the first pivot, solve the second equation for $x_2$, and substitute into the first equation to find $x_1$.

Gaussian elimination is simpler for this right-hand side because one row operation and back substitution give the solution directly.
