### Exercise 11. When Do Matrices Commute?
Given

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}.
$$

Find the conditions on $a,b,c,d$ under which $AB=BA$. Describe the general form of all such matrices $B$.

> **Why this exercise:** deepens the idea of noncommutativity by finding the conditions under which commutativity does hold.

#### Solution

Multiplication by rows and columns gives

$$
AB=
\begin{pmatrix}
a+c & b+d \\
c & d \\
\end{pmatrix},
\qquad BA=
\begin{pmatrix}
a & a+b \\
c & c+d \\
\end{pmatrix}.
$$

The upper-left entries agree exactly when $c=0$. The upper-right entries agree exactly when $d=a$. The lower-left entries already agree, and the lower-right entries give the same condition $c=0$. Thus the matrices that commute with $A$ are exactly

$$
B=
\begin{pmatrix}
a & b \\
0 & a \\
\end{pmatrix},
\qquad a,b\in\mathbb{R}.
$$

**Verification.** Substituting $c=0$ and $d=a$ into both products gives

$$
AB=BA=
\begin{pmatrix}
a & a+b \\
0 & a \\
\end{pmatrix}.
$$
