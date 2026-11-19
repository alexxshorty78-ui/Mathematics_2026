## Exercise 10. Columns of a Matrix Product

### Question

Given:

$$
A = \begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix}, \quad
B = \begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1 \\
\end{pmatrix}
$$

Denote the columns of $B$ by $b_1, b_2$.
1. Compute $Ab_1$ and $Ab_2$.
2. Compute the matrix $AB$.
3. Compare the results and explain why the columns of $AB$ are exactly the vectors $Ab_1$ and $Ab_2$.

*Why this exercise:* extends the interpretation of matrix-vector multiplication to a full product of two matrices instead of simply repeating another $Ax$ exercise.

---

### Solution

#### 1. Computing $Ab_1$ and $Ab_2$
First, let's identify the columns of matrix $B$:

$$
b_1 = \begin{pmatrix}
1 \\
-1 \\
3 \\
\end{pmatrix}, \quad b_2 = \begin{pmatrix}
2 \\
0 \\
1 \\
\end{pmatrix}
$$

* **Computing $Ab_1$:**

$$
Ab_1 = \begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix} \begin{pmatrix}
1 \\
-1 \\
3 \\
\end{pmatrix} = \begin{pmatrix}
(1)(1) + (2)(-1) + (0)(3) \\
(0)(1) + (1)(-1) + (1)(3) \\
\end{pmatrix} = \begin{pmatrix}
1 - 2 + 0 \\
0 - 1 + 3 \\
\end{pmatrix} = \begin{pmatrix}
-1 \\
2 \\
\end{pmatrix}
$$

* **Computing $Ab_2$:**

$$
Ab_2 = \begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix} \begin{pmatrix}
2 \\
0 \\
1 \\
\end{pmatrix} = \begin{pmatrix}
(1)(2) + (2)(0) + (0)(1) \\
(0)(2) + (1)(0) + (1)(1) \\
\end{pmatrix} = \begin{pmatrix}
2 + 0 + 0 \\
0 + 0 + 1 \\
\end{pmatrix} = \begin{pmatrix}
2 \\
1 \\
\end{pmatrix}
$$

#### 2. Computing the Matrix $AB$
Multiplying matrices $A_{2 \times 3}$ and $B_{3 \times 2}$ directly:

$$
AB = \begin{pmatrix}
(1)(1) + (2)(-1) + (0)(3) & (1)(2) + (2)(0) + (0)(1) \\
(0)(1) + (1)(-1) + (1)(3) & (0)(2) + (1)(0) + (1)(1) \\
\end{pmatrix} = \begin{pmatrix}
-1 & 2 \\
2 & 1 \\
\end{pmatrix}
$$

#### 3. Comparison and Explanation
The vectors from part 1 match the first and second columns of $AB$, respectively.

The entry in row $i$ and column $j$ of $AB$ is the dot product of row $i$ of $A$ and column $b_j$ of $B$. The same dot product gives entry $i$ of the vector $Ab_j$, so column $j$ of $AB$ is $Ab_j$.
