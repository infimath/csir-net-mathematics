---
layout: post
title: Problems on Minimal Polynomials
tags: [Minimal Polynomials]
---

**Question 1:** Let $f(x)$ be the minimal polynimial of the $4\times 4$ matrix
$$A=\begin{pmatrix}0 & 0 & 0 & 1 \\ 1 & 0 & 0 & 0 \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 1 & 0 \end{pmatrix}. $$
Then the rank of the $4\times 4$ matrix $f(A)$ is
1. $0$   2. $1$   3. $2$    4. $4$

**Answer:** Minimal polynomial is smallest degree polynomial satisfies the matrix. Hence $f( A) = 0$.

Hence option **1** is correct.

****
**Question 2:** Let $V$ and $W$ be finite dimensional vector spaces over   $\mathbb{R}$ and let $T_1:V \rightarrow V$ and $T_2:V \rightarrow V$  be the linear transformation whose minimal polynomials are given by
$$f_1(x)=x^2+x^2+x+1 \text{ and } f_2(x)=x^4-x^2-2.$$
Let $T:V\oplus W \rightarrow V \oplus W$  be the linear transformation defined by
$$T(v,w)=(T_1(v),T_2(w)) \text{ for } (v,w)\in V\oplus W $$
and let $f(x)$ be the minimal polynomial of $T$. Then

1. $\deg f(x)=7$
2. $\deg f(x)=5$
3. nullity $T=1$
4. nullity $T=0$

**Answer:** The Minimum polynomial of
$$T : V_1 \oplus V_2 \oplus \cdots \oplus V_n \rightarrow V_1 \oplus V_2 \oplus \cdots \oplus V_n$$
will  be the least common multiple of the minimum polynomials of $T_{V_i} : V_i \rightarrow V_i$, where $T_{V_i}$ is restriction of the function $T$ on subspace $V_i$.
Here,
$$\begin{align*} f_1(x) &= x^3+x^2+x+1 \\&= (x^2 + 1)(x+1)\\ f_2( x) &= x^4-x^2-2 \\&= (x^4 - 1) - (x^2 +1) \\&= (x^2 +1)(x^2-2) \end{align*}$$
Hence [$f_1(x), f_2( x)$] = $(x^2 + 1)(x+1)(x^2-2)$, which has degree $5$. Also minimal polynomial has a constant term, hence $T$ is invertible. Hence nullity $T=0$.

Hence options **2 and 4** are correct.
