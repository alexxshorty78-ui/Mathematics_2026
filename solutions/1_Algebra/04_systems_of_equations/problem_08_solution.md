# Exercise 8. Two Systems with the Same Coefficient Matrix

## Question

Solve by elimination the two systems

$$
\begin{cases}
2x+y=5, \\
x-y=1, \\
\end{cases}
$$

$$
\begin{cases}
2x+y=1, \\
x-y=4. \\
\end{cases}
$$

Compare the successive elimination steps. Which part of the calculation is the same in both cases, and why?

## Solution

Both systems have coefficient matrix

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & -1 \\
\end{pmatrix}.
$$

### First system

Swap the rows to use a leading coefficient of $1$, then apply $R_2\leftarrow R_2-2R_1$:

$$
\begin{pmatrix}
2 & 1 & \mid & 5 \\
1 & -1 & \mid & 1 \\
\end{pmatrix}
\xrightarrow{R_1\leftrightarrow R_2}
\begin{pmatrix}
1 & -1 & \mid & 1 \\
2 & 1 & \mid & 5 \\
\end{pmatrix}
\xrightarrow{R_2\leftarrow R_2-2R_1}
\begin{pmatrix}
1 & -1 & \mid & 1 \\
0 & 3 & \mid & 3 \\
\end{pmatrix}.
$$

Thus $y=1$ and $x-y=1$ gives $x=2$:

$$
(x,y)=(2,1).
$$

Check: $2(2)+1=5$ and $2-1=1$.

### Second system

Use exactly the same row operations:

$$
\begin{pmatrix}
2 & 1 & \mid & 1 \\
1 & -1 & \mid & 4 \\
\end{pmatrix}
\xrightarrow{R_1\leftrightarrow R_2}
\begin{pmatrix}
1 & -1 & \mid & 4 \\
2 & 1 & \mid & 1 \\
\end{pmatrix}
\xrightarrow{R_2\leftarrow R_2-2R_1}
\begin{pmatrix}
1 & -1 & \mid & 4 \\
0 & 3 & \mid & -7 \\
\end{pmatrix}.
$$

Thus $y=-7/3$ and $x-y=4$ gives $x=4-7/3=5/3$:

$$
(x,y)=\left(\frac53,-\frac73\right).
$$

Check:

$$
2\left(\frac53\right)-\frac73=1,
\qquad
\frac53-\left(-\frac73\right)=4.
$$

### Comparison

The row swap, elimination multiplier $2$, and resulting triangular coefficient matrix are identical. They depend only on $A$. The right-hand sides differ, so their transformed entries and the final solutions differ. The coefficient-side elimination can therefore be reused, provided the same operations are also applied to each right-hand side.
