### Exercise 9. Composing Transformations

Let

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix},\qquad R=
\begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix}.
$$

The matrix $S$ describes nonuniform scaling, while $R$ describes a $90^\circ$ counterclockwise rotation.
For

$$
x=
\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}
$$

compute $RSx$ and $SRx$. Compare the results and explain geometrically why the order of these transformations matters.

> **Why this exercise:** interprets matrix multiplication as composition of transformations.

#### Solution

The product $RSx$ means $R(Sx)$: the transformation $S$ is applied first, then $R$. Likewise $SRx$ means $S(Rx)$: first $R$, then $S$.

**Computation of $RSx$**

First apply $S$ to $x$:

$$
Sx=
\begin{pmatrix}
2\cdot1+0\cdot2 \\
0\cdot1+1\cdot2 \\
\end{pmatrix}
$$

Hence

$$
Sx=
\begin{pmatrix}
2 \\
2 \\
\end{pmatrix}
$$

Now apply $R$:

$$
R(Sx)=
\begin{pmatrix}
0\cdot2+(-1)\cdot2 \\
1\cdot2+0\cdot2 \\
\end{pmatrix}
$$

Hence

$$
RSx=
\begin{pmatrix}
-2 \\
2 \\
\end{pmatrix}
$$

**Computation of $SRx$**

First apply $R$ to $x$:

$$
Rx=
\begin{pmatrix}
0\cdot1+(-1)\cdot2 \\
1\cdot1+0\cdot2 \\
\end{pmatrix}
$$

Hence

$$
Rx=
\begin{pmatrix}
-2 \\
1 \\
\end{pmatrix}
$$

Now apply $S$:

$$
S(Rx)=
\begin{pmatrix}
2\cdot(-2)+0\cdot1 \\
0\cdot(-2)+1\cdot1 \\
\end{pmatrix}
$$

Hence

$$
SRx=
\begin{pmatrix}
-4 \\
1 \\
\end{pmatrix}
$$

**Verification through the products of matrices**

The product of the matrices gives the same results:

$$
RS=
\begin{pmatrix}
0 & -1 \\
2 & 0 \\
\end{pmatrix},\qquad SR=
\begin{pmatrix}
0 & -2 \\
1 & 0 \\
\end{pmatrix}.
$$

Then

$$
RSx=
\begin{pmatrix}
0\cdot1+(-1)\cdot2 \\
2\cdot1+0\cdot2 \\
\end{pmatrix}=
\begin{pmatrix}
-2 \\
2 \\
\end{pmatrix},
$$

$$
SRx=
\begin{pmatrix}
0\cdot1+(-2)\cdot2 \\
1\cdot1+0\cdot2 \\
\end{pmatrix}=
\begin{pmatrix}
-4 \\
1 \\
\end{pmatrix}.
$$

**Comparison**

The results differ:

$$
RSx\neq SRx.
$$

Consequently $RS\neq SR$, which is another instance of noncommutativity of matrix multiplication.

**Geometric explanation**

The scaling $S$ stretches the plane only in the direction of the $x_1$-axis, by the factor $2$, and leaves the $x_2$-direction unchanged. It is therefore not symmetric with respect to rotation: it distinguishes the horizontal direction from the vertical one.

- In $RSx$, the vector is stretched horizontally first, from $(1,\,2)$ to $(2,\,2)$, and the stretched vector is then rotated by $90^\circ$. The stretch acts along the original horizontal direction, and the rotation carries the result to $(-2,\,2)$.
- In $SRx$, the vector is rotated first, from $(1,\,2)$ to $(-2,\,1)$, and the rotated vector is then stretched horizontally. The stretch now acts on the rotated vector, whose horizontal component is $-2$, so it becomes $-4$ and the vertical component stays $1$.

In the first case the stretching is applied along the original horizontal direction and then rotated together with the vector. In the second case the stretching is applied along the horizontal direction after the rotation, that is, along the direction that was originally vertical. These are different directions relative to the vector, so the final vectors differ.

A rotation commutes with a scaling only when the scaling is uniform, that is, when it has the form $cI$. Here the scaling factors $2$ and $1$ differ, so the order of the transformations matters.

**Conclusion**

The product $RS$ represents the transformation "first scale, then rotate", and $SR$ represents "first rotate, then scale". Matrix products are read from right to left, since the matrix nearest to the vector acts first.