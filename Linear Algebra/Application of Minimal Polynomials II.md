---
layout: post
title: Application of Minimal Polynomials II
tags: [Matrix, Minimal Polynomials, Trace]
---

**Question 1:** For a fixed positive integer $n \geq 3$ , Let $A$ be the $n\times n$ matrix defined as $A=I-\frac{1}{n}J$, where is the $n\times n$  matrix with all entries equal to $1$. Which of the following statements is NOT true?

1. $A^k=A$ for every positive integer $k$.
2. trace $A=n-1$
3. rank $(A)-$ rank $ (I-A)=n$
4. $A$ is invertible

**Answer:** Note that $J^2 = nJ$, applying this we get
\begin{align*} A^2 &= \left(I-\frac{1}{n}J \right)^2 \\ &= I^2 - 2\cdot I \cdot \frac{1}{n}J + J^2 \\ &= I^2  - \frac{2}{n}J + nJ \\ &= I-\frac{1}{n}J \\&= A \end{align*}
Using this we get $A^k=A$ for every positive integer $k$, $i.e.$, option 1 is correct.
Also,
\begin{align*} A &= I-\frac{1}{n}J \\ \Rightarrow \mbox{trace }A &= \mbox{trace } I - \mbox{trace } \left(\frac{1}{n}J \right) \\ &= n - \frac{1}{n}n \\&= n-1\end{align*}
Hence option 2 is also correct.
Since we have seen that $A^2 = A$, we get  the minimal polynomial of $A$ is $x^2-x = x(x -1)$. Clearly it has one eigenvalue $0$. The matrix $A$ is not invertible. Hence option 4 is wrong.
Also note that $A$ is not invertible implies that rank $A < n$. Hence option 3 is wrong because rank of any matrix can’t be negative.

Combining all, options **3 and 4** is correct.

*****
**Question 2:**  Let $T$ be a linear transformation on the real vector space $\mathbb{R}^n$ over $\mathbb{R}$ such that $T^2=\lambda T$ for some $\lambda \in \mathbb{R}$. Then

1.   $\Vert Tx \Vert = \vert \lambda \vert \Vert x \Vert$ for all $x\in \mathbb{R}^n$.
2.   $\Vert Tx \Vert =  \Vert x \Vert$ for some nonzero vector $x\in \mathbb{R}^n$, then $\lambda =\pm 1$.
3.   $T=\lambda I$ where $I$ is the identity transformation on $\mathbb{R}^n$.
4.   $\Vert Tx \Vert >  \Vert x \Vert$ for some nonzero vector $x\in \mathbb{R}^n$, then $T$ is necessarily singular.

**Answer:**  The matrix of linear transformation $T$ satisfies $T^2=\lambda T$, hence it’s minimal polynomial will be a factor of $x^2 - \lambda x = x(x-\lambda)$. Hence the minimal polynomial can be $x,$ $(x-\lambda)$ or $x(x-\lambda)$. In all these cases, the matrix will be diagonalizable with eigenvalues $0$ or $\lambda $ or both.

*Option 1:* is correct if we take $\lambda = 0$, We get $T x = 0 = 0.x$ for all $x \in \mathbb{R}^n$

*Option 2:* is also correct for $x$ belonging to eigenspace of  $\lambda$

*Option 3:* is certainly wrong because there is one subspace belong to eigenspace say $E_0$ of $0$ such that $Tx = 0 $ for all $x \in E_0$

*Option 4:* is correct without any extra condition on $T$ as $0$ is a eigenvalue of $T$, hence it has to be singular.

Combining all we get **1, 2 and 4** are correct options.

*****
**Question 3:**  Let $A$ be a $4 \times 4$ matrix over $ \mathbb{C}$ such that rank$(A) = 2$ and $A^3 = A^2 \neq 0$. Suppose that $A$ is not diagonalizable. Then

1.  One of the Jordan blocks of the Jordan canonical form of $A$ is $\begin{pmatrix} 0 & 1 \\ 0 & 0 \end{pmatrix}$
2.  $A^2 = A \neq 0 $
3.  There exists a vector $v$ such that $Av \neq 0$ but $A^2 v = 0$
4.  The characteristic polynomial of $A$ is $x^4 - x^3$

**Answer:** The matrix satisfies the equation $A^3 = A^2$, hence it’s minimal polynomial will be a factor of $x^3-x^2 = x^2(x-1)$.

>It is given that the matrix is non-diagonalizable, hence it's minimal polynomial will have **al-least** one factor with multiplicity greater than $1$.

Hence the minimal polynomial will be either $x^2$ or $x^2(x-1)$. Now let's write possible $4\times  4$ matrices with the above minimal polynomials.

First consider, $x^2$, then all $4\times 4$ matrices with this minimal polynomial are
$$ A_1 = \begin{bmatrix} 0 & 1 &&\\ 0 & 0 &&\\ && 0 & \\ &&&0  \end{bmatrix}\quad \text{and}\quad A_2 = \begin{bmatrix} 0 & 1 &&\\ 0 & 0 &&\\ && 0 & 1\\ &&&0  \end{bmatrix}$$

Also, all $4\times 4$ matrices with the minimal polynomial $x^2(x-1)$ is
$$A_3=\begin{bmatrix} 0 & 1 &&\\ 0 & 0 &&\\ && 0 & \\ &&&1  \end{bmatrix}\quad \text{and}\quad A_4 = \begin{bmatrix} 0 & 1 &&\\ 0 & 0 &&\\ && 1 & \\ &&&1  \end{bmatrix}$$

Out of these four matrices $A_2$ and $A_3$ have rank $2$.  But $A_2^2 = 0$, hence we are left with $A_3$ only. It's characteristic polynomial will be $x^3(x-1)=x^4-x^3$. It also has a generalized eigenvector corresponds to eigenvalue $0$.

Since, $A_3^2 \neq A_3$, hence choice 2 is incorrect.

Hence **1, 3 and 4** are correct.

*****
**Question 4:** Which of the following matrices have Jordan Canonical form equal to
$$\begin{pmatrix} 0 & 1 & 0 \\ 0 & 0 & 0 \\ 0 & 0 & 0 \end{pmatrix}?$$
$$
\begin{align*} &1. \begin{pmatrix} 0 & 0 & 1 \\ 0 & 0 & 0 \\ 0 & 0 & 0 \end{pmatrix} &2.  \begin{pmatrix} 0 & 0 & 1 \\ 0 & 0 & 1 \\ 0 & 0 & 0 \end{pmatrix} \\
&3. \begin{pmatrix} 0 & 1 & 1 \\ 0 & 0 & 0 \\ 0 & 0 & 0 \end{pmatrix} &4.  \begin{pmatrix} 0 & 1 & 1 \\ 0 & 0 & 1 \\ 0 & 0 & 0 \end{pmatrix} \end{align*}$$

**Answer:** Two similar matrices have same Jordan form.

> When the multiplicity of each root of characteristic polynomial is at most three, Jordan form can be uniquely identified by it’s minimal polynomial.

Here the characteristic polynomial of all given matrices are $x^3$. Hence the Jordan form can be completely characterized by it’s minimal polynomial. The matrix in problem is in Jordan form hence we can quickly tell it’s minimal polynomial, $i.e.$,  $x^2$. Now compute the minimal polynomial of the matrices given in option.
**Option 1,2 and 3:** $A^2 = 0$, hence minimal polynomial is $x^2$.
**Option 4:** $A^2 \neq 0$, hence minimal polynomial will $x^3$.

Hence **1, 2 and 3** are correct.
