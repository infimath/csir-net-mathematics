---
layout: post
title: Questions Based on System of Linear Equation
tags: [Linear Equation]
---


**Question 1:** The system of equations
$$
\begin{align*} x+y+z=1\\ 2x+3y-z=5\\ x+2y-kz=4\end{align*}
$$
Where $k\in \mathbb{R}$, has an infinite number of solutions for

 1. $k=0$  2. $k=1$  3. $k=2$  4. $k=3$

**Answer:** Rank of augmented matrix and coefficient matrix can decide the number of solution of a linear system.
> A system of linear equation has infinitely many solution if and only $$\text{rank }\tilde{A} = \text{rank }A < n ,$$  where  $\tilde{A}$ is the augmented matrix of the given system of linear equation.

Here,
$$ \left [ \begin{array}{ccc|c} 1 & 1 & 1 & 1 \\ 2 & 3 & -1 & 5 \\ 1 & 2 & -k & 4 \end{array} \right ] \xrightarrow{\text{Convert to EF}} \left [ \begin{array}{ccc|c} 1 & 1 & 1 & 1 \\ 0 & 1 & -3 & 3 \\ 0 & 0 & 2-k & 0 \end{array} \right]$$

Now to fulfil the condition of infinitely many solution as stated above $2 - k = 0 \Rightarrow k = 2$.
Hence option **3** is correct.

*******
**Question 2:** Let $A$ be a $5\times 4$ matrix with real entries such that $Ax=0$ if and only if $x=0$ where $x$ is a $4\times 1$ vector and $0$ is a null vector. Then, the rank of $A$ is

1. $4$  2. $5$  3. $2$   4.$1$

**Answer:** The condition of unique solution is applicable here
> A system of linear equation has unique solution if and only if
> $$\text{rank}\tilde{A}= \text{rank }A = n.$$

Here, the $n = 4$ and hence rank is also $4$.

Hence option **1** is correct.

****
**Question 3:**  Let $A$ be a $5\times 4$ matrix with real entries such that the space of all solutions of the linear system $AX^t=[1,2,3,4,5]^t$ is given by $\{[1+2s,2+3s,3+4s,4+5s]^t:s \in \mathbb{R} \}.$ Then the rank of $A$ is equal to

1. $4$  2. $3$  3. $2$   4. $1$

**Answer:** Here solution consist of one parameter. Hence the system of linear equation has one free variable.
$$
\begin{align}
\rm{rank}~A &= \# \text{Pivot variable} \\
&= n-\#\text{Free variable} \\
&= 4-1 = 3.
\end{align}
$$

Hence option **2** is correct.

*****
**Question 4:**  Consider a homogeneous system of linear equation $Ax = 0$ where $A$ is an $m \times n$ real matrix and $n>m$. Then which of the following statements are always true?

1. $Ax = 0$ has a solution.
2. $Ax = 0$ has no non-zero  solution .
3. $Ax = 0$ has a non-zero solution.
4. Dimension of the space of all solution is at least $n-m$

**Answer:** This is a theoretical question. As we know a homogeneous system of linear equation with more unknown than constrain has infinitely many solution. If the matrix $A$ has maximum rank $m = \min\{m,n\}$. Then dimension of solution space will be at least $n - m$.

Hence option **1, 3 and 4** are correct.
