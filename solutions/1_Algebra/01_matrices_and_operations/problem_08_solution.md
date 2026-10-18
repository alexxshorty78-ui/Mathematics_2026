### Exercise 8. Row Operations and Their Reversibility

For

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3 \\
\end{pmatrix}
$$

perform, in order:

1. $R_2\leftarrow R_2-2R_1$,
2. $R_3\leftarrow R_3+R_1$,
3. interchange $R_2$ and $R_3$.

Write the matrix after each step. Then, for each of the three operations, state an operation that reverses it.

> **Why this exercise:** prepares for elimination by showing that row operations are controlled and reversible transformations of a matrix.

#### Solution

**Step 1: $R_2\leftarrow R_2-2R_1$**

The new second row is

$$
(2,\,4,\,1)-2(1,\,2,\,-1)=(0,\,0,\,3).
$$

The first and third rows are unchanged. Hence

$$
A_1=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3 \\
\end{pmatrix}
$$

**Step 2: $R_3\leftarrow R_3+R_1$**

The new third row is

$$
(-1,\,1,\,3)+(1,\,2,\,-1)=(0,\,3,\,2).
$$

The first and second rows are unchanged. Hence

$$
A_2=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2 \\
\end{pmatrix}
$$

**Step 3: interchange $R_2$ and $R_3$**

The second and third rows exchange places. Hence

$$
A_3=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3 \\
\end{pmatrix}
$$

The matrix $A_3$ is upper triangular, so the three operations have brought $A$ to a form suitable for back substitution.

**Reversing operations**

| Operation | Reversing operation |
|---|---|
| $R_2\leftarrow R_2-2R_1$ | $R_2\leftarrow R_2+2R_1$ |
| $R_3\leftarrow R_3+R_1$ | $R_3\leftarrow R_3-R_1$ |
| interchange $R_2$ and $R_3$ | interchange $R_2$ and $R_3$ |

Adding a multiple of one row to another is undone by adding the opposite multiple of the same row, and this is possible because the row $R_1$ used in the operation is not changed by it. A row interchange is its own reverse, since performing it twice restores the original order.

**Verification**

The reversing operations must be applied in the opposite order: first the interchange, then the reverse of Step 2, then the reverse of Step 1.

Interchanging $R_2$ and $R_3$ in $A_3$ gives

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2 \\
\end{pmatrix}=A_2.
$$

Applying $R_3\leftarrow R_3-R_1$ gives the third row $(0,\,3,\,2)-(1,\,2,\,-1)=(-1,\,1,\,3)$, so

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3 \\
\end{pmatrix}=A_1.
$$

Applying $R_2\leftarrow R_2+2R_1$ gives the second row $(0,\,0,\,3)+2(1,\,2,\,-1)=(2,\,4,\,1)$, so

$$
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3 \\
\end{pmatrix}=A.
$$

The original matrix is recovered.

**Conclusion**

Each of the three row operations can be undone by another row operation of the same kind. Therefore no information about $A$ is lost during elimination, and a sequence of row operations can always be reversed by undoing its steps in the opposite order.