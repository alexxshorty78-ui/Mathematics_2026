### Exercise 3. When Can Matrices Be Multiplied?

The matrix sizes are

$$
A_{2\times3},\qquad B_{3\times4},\qquad C_{4\times2},\qquad D_{2\times2}.
$$

For the products

$$
AB,\ BA,\ BC,\ CB,\ AC,\ CA,\ AD,\ DA
$$

determine whether they are defined. If so, state the size of the result. Justify each decision using the dimension compatibility condition.

> **Why this exercise:** forces an understanding of dimension compatibility before carrying out any calculation.

#### Solution

**Compatibility condition**

Let $X$ be of size $m\times n$ and $Y$ of size $p\times q$. The product $XY$ is defined if and only if

$$
n=p,
$$

that is, the number of columns of $X$ equals the number of rows of $Y$. In that case $XY$ has size $m\times q$.

**Product $AB$**

Here $A$ is $2\times3$ and $B$ is $3\times4$. The inner dimensions are $3$ and $3$, which agree. The product $AB$ is defined and has size $2\times4$.

**Product $BA$**

Here $B$ is $3\times4$ and $A$ is $2\times3$. The inner dimensions are $4$ and $2$, which differ. The product $BA$ is not defined.

**Product $BC$**

Here $B$ is $3\times4$ and $C$ is $4\times2$. The inner dimensions are $4$ and $4$, which agree. The product $BC$ is defined and has size $3\times2$.

**Product $CB$**

Here $C$ is $4\times2$ and $B$ is $3\times4$. The inner dimensions are $2$ and $3$, which differ. The product $CB$ is not defined.

**Product $AC$**

Here $A$ is $2\times3$ and $C$ is $4\times2$. The inner dimensions are $3$ and $4$, which differ. The product $AC$ is not defined.

**Product $CA$**

Here $C$ is $4\times2$ and $A$ is $2\times3$. The inner dimensions are $2$ and $2$, which agree. The product $CA$ is defined and has size $4\times3$.

**Product $AD$**

Here $A$ is $2\times3$ and $D$ is $2\times2$. The inner dimensions are $3$ and $2$, which differ. The product $AD$ is not defined.

**Product $DA$**

Here $D$ is $2\times2$ and $A$ is $2\times3$. The inner dimensions are $2$ and $2$, which agree. The product $DA$ is defined and has size $2\times3$.

**Summary**

| Product | Sizes | Inner dimensions agree? | Result size |
|---|---|---|---|
| $AB$ | $2\times3$, $3\times4$ | yes | $2\times4$ |
| $BA$ | $3\times4$, $2\times3$ | no | not defined |
| $BC$ | $3\times4$, $4\times2$ | yes | $3\times2$ |
| $CB$ | $4\times2$, $3\times4$ | no | not defined |
| $AC$ | $2\times3$, $4\times2$ | no | not defined |
| $CA$ | $4\times2$, $2\times3$ | yes | $4\times3$ |
| $AD$ | $2\times3$, $2\times2$ | no | not defined |
| $DA$ | $2\times2$, $2\times3$ | yes | $2\times3$ |

The defined products are $AB$, $BC$, $CA$, and $DA$. Note that $AB$ is defined while $BA$ is not, and likewise for $BC$ and $CB$. Matrix multiplication is therefore not commutative in general, since one order of a product may exist while the other does not.