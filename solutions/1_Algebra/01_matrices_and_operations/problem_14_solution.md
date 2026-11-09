### Exercise 14. Rotation Matrices
The matrix for a rotation through an angle $\theta$ is

$$
R(\theta)=
\begin{pmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta \\
\end{pmatrix}.
$$

Compute $R(\alpha)R(\beta)$ and, using the angle-sum formulas for sine and cosine, show that

$$
R(\alpha)R(\beta)=R(\alpha+\beta).
$$

Explain the result geometrically.

> **Why this exercise:** shows the consistency between matrix algebra and the geometry of composing rotations.

#### Solution

Multiplication by rows and columns gives

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha\cos\beta-\sin\alpha\sin\beta & -\cos\alpha\sin\beta-\sin\alpha\cos\beta \\
\sin\alpha\cos\beta+\cos\alpha\sin\beta & \cos\alpha\cos\beta-\sin\alpha\sin\beta \\
\end{pmatrix}.
$$

The angle-sum formulas are

$$
\begin{aligned}
\cos(\alpha+\beta) &= \cos\alpha\cos\beta-\sin\alpha\sin\beta \\
\sin(\alpha+\beta) &= \sin\alpha\cos\beta+\cos\alpha\sin\beta.
\end{aligned}
$$

Substituting these expressions into the product yields

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos(\alpha+\beta) & -\sin(\alpha+\beta) \\
\sin(\alpha+\beta) & \cos(\alpha+\beta) \\
\end{pmatrix}
= R(\alpha+\beta).
$$

For a vector $v$, the product applies $R(\beta)$ first and then $R(\alpha)$. Both rotations are about the origin. The length of $v$ is preserved, and the direction of a nonzero $v$ changes by $\beta+\alpha$, the same change produced by a single rotation through $\alpha+\beta$.
