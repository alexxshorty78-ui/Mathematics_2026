# Exercise 14. A Small Change in the Right-Hand Side

## Question

Compare the systems

$$
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3 \\
\end{cases}
$$

and

$$
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3.1. \\
\end{cases}
$$

Check the consistency of each system and explain why a small change in one number can change the type of the system.

## Solution

Adding the first two equations gives $3x=3$. Therefore $x=1$, and substituting into the first equation gives $y=1$. The second equation is also satisfied since $2(1)-1=1$.

**First system.** The third equation agrees with the consequence $3x=3$. The system is consistent and has the unique solution $(1,1)$.

**Second system.** The same first two equations still force $3x=3$. The third requires $3x=3.1$, so subtracting their consequence from the third equation gives

$$
0=3.1-3=0.1.
$$

The system is inconsistent. The third left-hand side is the sum of the first two, so consistency requires the corresponding right-hand sides to add up exactly.
