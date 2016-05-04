---
layout: post
title: CSIR-NET December 2015 Linear Algebra(Part B)
tags: [2015, Determinant, Trace, Linear Transformation, Minimal Polynomials, Quadratic Forms]
---

**Question 1:** If $A$ is a $5\times 5$ real matrix with trace $15$ and if $2$ and $3$ are eigenvalues of $A$ , each with algebraic multiplicity $2$, then the determinant of $A$ is equal to

1. $0$
2. $24$
3. $120$
4. $180$

**Answer:** Out of five eigenvalues of matrix $A$ we know four $2,~2,~3,~3$. Let the last eigenvalue is $\lambda$. Then,
$$\begin{align}& \text{ trace }A = 2+2+3+3+\lambda\\ \Rightarrow& \lambda = 15-10=5.\end{align}$$
Hence the determinant, will be product of eigenvalues
$$\text{ det }A = 2\cdot 2\cdot 3\cdot 3\cdot 5=180.$$

Hence **4** is correct choice.

***
**Question 2:** For a positive integer $n$, let $P_n$ denote the vector space of polynomials in one variable $x$ with real coefficients and with degree $\leq n$. Consider the map $T:P_2 \rightarrow P_4$ defined by $T(p(x)) = p(x^2)$. Then

1. $T$ is a linear transformation and dim range $(T) = 5$.
2. $T$ is a linear transformation and dim range $(T) = 3$.
3. $T$ is a linear transformation and dim range $(T) = 2$.
4. $T$ is not a linear transformation.

**Answer:** This transformation replaces each $x$ by $x^2$. Also,
$$\begin{align}T(\alpha p(x) + \beta q(x)) &= \alpha p(x^2) + \beta q(x^2)\\ &=\alpha T(p(x)) + \beta T(q(x))\end{align}$$
Hence this is a linear transformation, and
$$\text{ ker }T = \{p(x) : p(x^2) = 0\} = \{0\}.$$
Hence the nullity will be zero. By rank nullity theorem, we get
$$
\begin{align}
\text{ rank }T &= \text{ dim }P_2 - \text{ nullity }\\
&= 3 - 0 \\
&= 3
\end{align}
$$

Hence **2** is correct choice.

***
**Question 3:** Let $A$ be a real $3\times 4$ matrix of rank $2$. Then the rank of $A^tA$, where $A^t$ deonotes the transpose $A$, is

1. exactly $2$
2. exactly $3$
3. exactly $4$
4. at most $2$ but not necessarily $2$

**Answer:** Given that the rank of $A$ is $2$, hence the nullity of $A$ is $4-2 = 2$. Using theorem,
> Nullspace of $A$ and $A^TA$ are the same.

We get the nullity of $A^TA$ is 2. Since $A^TA$ is $4\times 4$ matrix. Hence rank of $A^TA$ will be $4-2 = 2$.

Hence **1** is correct choice.

***
**Question 4:**  Let $S$ denote the set of all the prime numbers $p$ with the property that the matrix
$$
\pmatrix{91& 31 & 0\\ 29 & 31 & 0\\ 79 & 23 & 59}
$$
has an inverse in the field $\newcommand{\Z}{\mathbb{Z}}\Z/p\Z$. Then

1. $S = \{31\}$
2. $S = \{31, ~59\}$
3. $S = \{7, ~13, ~59\}$
4. $S$ is infinite

**Answer:** The matrix is singular, if it's determinant will be zero in that field.
$$\begin{align}\text{ det } &= 59\times 31(91-29) \\ &= 59\times 31 \times  31 \times 2.\end{align}$$
The determinant will be zero in $\Z_p$ only for $p=59, ~31, ~2$. For all other primes it will be non-zero.

Hence **4** is correct choice.


***
**Question 5:** Consider the quadratic form $Q(v) = v^tAv$, where
$$A = \pmatrix{1&0&0&0 \\ 0&1&0&0 \\ 0&0&0&1 \\ 0&0&0&1}, v= (x,y,z,w)$$
Then

1. $Q$ has rank $3$.
2. $xy+z^2 = Q(P(v))$ for some invertible $4 \times 4$ real matrix $P$.
3. $xy+y^2+ z^2 = Q(P(v))$ for some invertible $4\times 4$ real matrix $P$.
4. $x^2+y^2-zw = Q(P(v))$ for some invertible $4\times 4$ real matrix $P$.

**Answer:** Here,
$$Q(Pv) = (Pv)^tAPv = v^t(P^tAP)v $$
When $P$ is orthogonal, $A$ and $P^tAP$ both represent equivalent quadratic forms. Then the problem is reduced to find equivalent bilinear forms.


***
**Question 6:** Let $A \neq I_n$ be an $n \times n$ matrix such that $A^2 = A$, where $I_n$ is the identity matrix of order $n$. Which of the following statements is false?

1. $(I_n - A)^2 = I_n - A$.
2. trace $(A)=$ rank $(A)$.
3. rank $(A)$ + rank $(I_n-A)$ = n.
4. The eigenvalus of $A$ are each equal to $1$.

**Answer:** The matrix satisfies the polynomial $x^2 - x = 0\Rightarrow x(x-1) = 0$. Hence minimal polynomial is a factor of $x(x-1)$. Since this polynomial has linear factors, hence matrix is diagonalizable with eigenvalues $0$ or $1$ or both. Since $A \neq I$ then at least eigenvalues will be $0$.

Hence **4** is correct choice.
