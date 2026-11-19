# Exercise 4 – Gauss–Jordan

## Question

Find $A^{-1}$ using the Gauss–Jordan method for:

$$
A=\begin{pmatrix}
1&2 \\
3&5 \\
\end{pmatrix}
$$

Show the augmented matrix after each operation and explain why obtaining $I$ on the left gives the inverse on the right.

## Solution

### 1. Set Up the Augmented Matrix

Start with:

$$
[A|I]=
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
3 & 5 & \mid & 0 & 1 \\
\end{pmatrix}
$$

### 2. Apply Row Operations

Subtract 3 times Row 1 from Row 2:

$$
R_2\rightarrow R_2-3R_1
$$

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & -1 & \mid & -3 & 1 \\
\end{pmatrix}
$$

Multiply Row 2 by -1:

$$
R_2\rightarrow -R_2
$$

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}
$$

Subtract 2 times Row 2 from Row 1:

$$
R_1\rightarrow R_1-2R_2
$$

$$
\begin{pmatrix}
1 & 0 & \mid & -5 & 2 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}
$$

### 3. Find the Inverse

The left side is now the identity matrix.

Therefore:

$$
A^{-1}=
\begin{pmatrix}
-5&2 \\
3&-1 \\
\end{pmatrix}
$$

### 4. Explanation

Let $E$ be the product of the elementary matrices for the row operations, taken in the order in which they act. Applying these operations to both blocks gives

$$
E[A\mid I]=[EA\mid EI]=[EA\mid E].
$$

The left block is $I$, so $EA=I$. Each elementary matrix is invertible, so $E$ is invertible and $A=E^{-1}$. Thus the right block $E$ equals $A^{-1}$.

### 5. Conclusion

$$
AA^{-1}=I
$$

Therefore, the inverse matrix is:

$$
A^{-1}=
\begin{pmatrix}
-5&2 \\
3&-1 \\
\end{pmatrix}
$$
