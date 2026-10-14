# Matrices and Basic Operations: Solutions Guide

## Exercise 1: Matrix Size and Entries

### Given Matrices
$$A = \begin{pmatrix} 2 & -1 & 3 \\ 0 & 4 & 5 \end{pmatrix}, \quad B = \begin{pmatrix} 1 & 0 & -2 \\ 3 & 4 & 1 \end{pmatrix}$$

### Solutions
1. **Sizes of Matrices:**
   * **Matrix $A$:** $2 \times 3$ (2 rows and 3 columns).
   * **Matrix $B$:** $2 \times 3$ (2 rows and 3 columns).

2. **Reading Specific Entries:**
   * $a_{12} = -1$ (Row 1, Column 2 of $A$)
   * $a_{23} = 5$ (Row 2, Column 3 of $A$)
   * $b_{21} = 3$ (Row 2, Column 1 of $B$)
   * $b_{32}$ = **Undefined**, because matrix $B$ only has 2 rows; there is no 3rd row.

3. **Vectors from Rows and Columns:**
   * Second row of $A$ as a vector: $(0, 4, 5)$
   * First column of $B$ as a vector: $\begin{pmatrix} 1 \\ 3 \end{pmatrix}$

---

## Exercise 2: Addition and Scalar Multiplication

### Given Matrices
$$A = \begin{pmatrix} 1 & 2 \\ -1 & 3 \end{pmatrix}, \quad B = \begin{pmatrix} 4 & -2 \\ 0 & 5 \end{pmatrix}$$

### Solutions
1. **Matrix Addition ($A + B$):**
   $$A + B = \begin{pmatrix} 1+4 & 2+(-2) \\ -1+0 & 3+5 \end{pmatrix} = \begin{pmatrix} 5 & 0 \\ -1 & 8 \end{pmatrix}$$

2. **Matrix Subtraction ($A - B$):**
   $$A - B = \begin{pmatrix} 1-4 & 2-(-2) \\ -1-0 & 3-5 \end{pmatrix} = \begin{pmatrix} -3 & 4 \\ -1 & -2 \end{pmatrix}$$

3. **Scalar Multiplication and Combination ($3A - 2B$):**
   $$3A = \begin{pmatrix} 3(1) & 3(2) \\ 3(-1) & 3(3) \end{pmatrix} = \begin{pmatrix} 3 & 6 \\ -3 & 9 \end{pmatrix}$$
   $$2B = \begin{pmatrix} 2(4) & 2(-2) \\ 2(0) & 2(5) \end{pmatrix} = \begin{pmatrix} 8 & -4 \\ 0 & 10 \end{pmatrix}$$
   $$3A - 2B = \begin{pmatrix} 3-8 & 6-(-4) \\ -3-0 & 9-10 \end{pmatrix} = \begin{pmatrix} -5 & 10 \\ -3 & -1 \end{pmatrix}$$

---

## Exercise 3: When Can Matrices Be Multiplied?

### Given Sizes
* $A$ is $2 \times 3$
* $B$ is $3 \times 4$
* $C$ is $4 \times 2$
* $D$ is $2 \times 2$

### Solutions and Dimension Compatibility Analysis
* **$AB$ ($2\times3$ and $3\times4$):** Inner dimensions match ($3 = 3$). $\rightarrow$ **Defined**, Result size: **$2 \times 4$**
* **$BA$ ($3\times4$ and $2\times3$):** Inner dimensions do not match ($4 \neq 2$). $\rightarrow$ **Undefined**
* **$BC$ ($3\times4$ and $4\times2$):** Inner dimensions match ($4 = 4$). $\rightarrow$ **Defined**, Result size: **$3 \times 2$**
* **$CB$ ($4\times2$ and $3\times4$):** Inner dimensions do not match ($2 \neq 3$). $\rightarrow$ **Undefined**
* **$AC$ ($2\times3$ and $4\times2$):** Inner dimensions do not match ($3 \neq 4$). $\rightarrow$ **Undefined**
* **$CA$ ($4\times2$ and $2\times3$):** Inner dimensions match ($2 = 2$). $\rightarrow$ **Defined**, Result size: **$4 \times 3$**
* **$AD$ ($2\times3$ and $2\times2$):** Inner dimensions do not match ($3 \neq 2$). $\rightarrow$ **Undefined**
* **$DA$ ($2\times2$ and $2\times3$):** Inner dimensions match ($2 = 2$). $\rightarrow$ **Defined**, Result size: **$2 \times 3$**

---

## Exercise 4: Matrix Multiplication and Noncommutativity

### Given Matrices
$$A = \begin{pmatrix} 1 & 2 \\ 0 & 1 \end{pmatrix}, \quad B = \begin{pmatrix} 2 & 0 \\ 3 & 1 \end{pmatrix}$$

### Solutions
1. **Compute $AB$:**
   $$AB = \begin{pmatrix} 1(2)+2(3) & 1(0)+2(1) \\ 0(2)+1(3) & 0(0)+1(1) \end{pmatrix} = \begin{pmatrix} 2+6 & 0+2 \\ 0+3 & 0+1 \end{pmatrix} = \begin{pmatrix} 8 & 2 \\ 3 & 1 \end{pmatrix}$$

2. **Compute $BA$:**
   $$BA = \begin{pmatrix} 2(1)+0(0) & 2(2)+0(1) \\ 3(1)+1(0) & 3(2)+1(1) \end{pmatrix} = \begin{pmatrix} 2+0 & 4+0 \\ 3+0 & 6+1 \end{pmatrix} = \begin{pmatrix} 2 & 4 \\ 3 & 7 \end{pmatrix}$$

3. **Is $AB = BA$?**
   $$\begin{pmatrix} 8 & 2 \\ 3 & 1 \end{pmatrix} \neq \begin{pmatrix} 2 & 4 \\ 3 & 7 \end{pmatrix} \implies AB \neq BA$$

---

## Exercise 5: Matrix Times Vector

### Given
$$A = \begin{pmatrix} 2 & -1 \\ 1 & 3 \end{pmatrix}, \quad x = \begin{pmatrix} 4 \\ 2 \end{pmatrix}$$

### Solutions
1. **Compute $Ax$:**
   $$Ax = \begin{pmatrix} 2(4) + (-1)(2) \\ 1(4) + 3(2) \end{pmatrix} = \begin{pmatrix} 8 - 2 \\ 4 + 6 \end{pmatrix} = \begin{pmatrix} 6 \\ 10 \end{pmatrix}$$

2. **Express as a Linear Combination of Columns:**
   $$Ax = 4\begin{pmatrix} 2 \\ 1 \end{pmatrix} + 2\begin{pmatrix} -1 \\ 3 \end{pmatrix} = \begin{pmatrix} 8 \\ 4 \end{pmatrix} + \begin{pmatrix} -2 \\ 6 \end{pmatrix} = \begin{pmatrix} 6 \\ 10 \end{pmatrix}$$

---

## Exercise 6: Transpose

### Given
$$A = \begin{pmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{pmatrix}, \quad B = \begin{pmatrix} 1 & 0 \\ 2 & 1 \\ -1 & 3 \end{pmatrix}$$

### Solutions
1. **Transposes ($A^T$ and $B^T$):**
   $$A^T = \begin{pmatrix} 1 & 4 \\ 2 & 5 \\ 3 & 6 \end{pmatrix}, \quad B^T = \begin{pmatrix} 1 & 2 & -1 \\ 0 & 1 & 3 \end{pmatrix}$$

2. **Compute $AB$:**
   $$AB = \begin{pmatrix} 2 & 11 \\ 8 & 23 \end{pmatrix}$$

3. **Verify $(AB)^T = B^T A^T$:**
   $$(AB)^T = \begin{pmatrix} 2 & 8 \\ 11 & 23 \end{pmatrix}, \quad B^T A^T = \begin{pmatrix} 2 & 8 \\ 11 & 23 \end{pmatrix} \implies (AB)^T = B^T A^T$$

---

## Exercise 7: Identity Matrix, Zero Matrix, and Powers

### Given
$$A = \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix}, \quad I = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix}, \quad 0 = \begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix}$$

### Solutions
1. **Neutral Elements:** $AI = IA = A$ and $A + 0 = A$.
2. **Matrix Powers:**
   * $A^2 = \begin{pmatrix} 4 & 4 \\ 0 & 4 \end{pmatrix}$
   * $A^3 = \begin{pmatrix} 8 & 12 \\ 0 & 8 \end{pmatrix}$
3. **Observed Pattern:**
   $$A^n = \begin{pmatrix} 2^n & n \cdot 2^{n-1} \\ 0 & 2^n \end{pmatrix}$$

---

## Exercise 8: Row Operations and Their Reversibility

### Given Matrix
$$A = \begin{pmatrix} 1 & 2 & -1 \\ 2 & 4 & 1 \\ -1 & 1 & 3 \end{pmatrix}$$

### Solutions
1. **Step 1 ($R_2 \leftarrow R_2 - 2R_1$):**
   $$A_1 = \begin{pmatrix} 1 & 2 & -1 \\ 0 & 0 & 3 \\ -1 & 1 & 3 \end{pmatrix} \quad (\text{Reversed by: } R_2 \leftarrow R_2 + 2R_1)$$

2. **Step 2 ($R_3 \leftarrow R_3 + R_1$):**
   $$A_2 = \begin{pmatrix} 1 & 2 & -1 \\ 0 & 0 & 3 \\ 0 & 3 & 2 \end{pmatrix} \quad (\text{Reversed by: } R_3 \leftarrow R_3 - R_1)$$

3. **Step 3 (Interchange $R_2$ and $R_3$):**
   $$A_3 = \begin{pmatrix} 1 & 2 & -1 \\ 0 & 3 & 2 \\ 0 & 0 & 3 \end{pmatrix} \quad (\text{Reversed by: Interchanging } R_2 \text{ and } R_3 \text{ again})$$

---

## Exercise 9: Composing Transformations

### Given
$$S = \begin{pmatrix} 2 & 0 \\ 0 & 1 \end{pmatrix}, \quad R = \begin{pmatrix} 0 & -1 \\ 1 & 0 \end{pmatrix}, \quad x = \begin{pmatrix} 1 \\ 2 \end{pmatrix}$$

### Solutions
1. **$RSx$ (Scale first, then rotate):**
   $$RSx = \begin{pmatrix} -2 \\ 2 \end{pmatrix}$$
2. **$SRx$ (Rotate first, then scale):**
   $$SRx = \begin{pmatrix} -4 \\ 1 \end{pmatrix}$$
3. **Comparison:** Since $RSx \neq SRx$, the order of matrix transformations changes the final geometric outcome.

---

## Exercise 10: Columns of a Matrix Product

### Given
$$A = \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \end{pmatrix}, \quad B = \begin{pmatrix} 1 & 2 \\ -1 & 0 \\ 3 & 1 \end{pmatrix}$$

### Solutions
1. **Compute $Ab_1$ and $Ab_2$:**
   * $Ab_1 = \begin{pmatrix} -1 \\ 2 \end{pmatrix}$
   * $Ab_2 = \begin{pmatrix} 2 \\ 1 \end{pmatrix}$

2. **Compute Matrix $AB$:**
   $$AB = \begin{pmatrix} -1 & 2 \\ 2 & 1 \end{pmatrix}$$

3. **Explanation:** The columns of the product matrix $AB$ are precisely the results of multiplying matrix $A$ by each individual column of $B$ ($Ab_1$ and $Ab_2$).

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

### Exercise 12. Formula for a Matrix Power
Let

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}.
$$

Compute $A^2$, $A^3$, and $A^4$, and use them to formulate a conjecture for $A^n$. Then do not stop after checking one more case: assume the formula is true for $n$, multiply by $A$, and explain why you obtain exactly the formula for $n+1$.

> **Why this exercise:** teaches how to recognize a pattern and formulate a generalization from several computations.

### Exercise 13. A Recurrence Written in Matrix Form
Let

$$
F=
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}.
$$

Compute $F^2$, $F^3$, $F^4$, and $F^5$. Compare the numbers obtained with the sequence

$$
0,1,1,2,3,5,8,\ldots
$$

and describe the relationship you observe. Then compute

$$
F
\begin{pmatrix}
a \\
b \\
\end{pmatrix}
$$

and explain how this multiplication performs one recurrence step: it creates the sum of two consecutive terms and keeps one of them for the next step.

> **Why this exercise:** shows the connection between matrix powers and a simple numerical recurrence.

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

### Exercise 15. Associativity of Multiplication and Different Calculation Paths
Given

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix},\quad B=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix},\quad C=
\begin{pmatrix}
2 & 1 \\
0 & -1 \\
\end{pmatrix}.
$$

Compute $(AB)C$ and $A(BC)$. Compare the results and the number of intermediate operations. Explain what associativity of matrix multiplication means in this example.

> **Why this exercise:** reinforces associativity by comparing two mathematically equivalent calculation paths.
