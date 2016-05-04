---
layout: post
title: Application of Minimal Polynomials I
tags: [Minimal Polynomials]
---

**Question 1:** Which of the following matrices is not diagonalizable over $\mathbb{R}$?

$$
\begin{align*}&1. \begin{pmatrix} 1 & 1 & 0 \\ 0 & 2 & 0 \\ 0 & 0 & 2 \end{pmatrix}        &  2. \begin{pmatrix} 1 & 1 & 0 \\ 0 & 2 & 1 \\ 0 & 0 & 3  \end{pmatrix} & \\ &3. \begin{pmatrix} 1 & 1 & 0 \\ 0 & 1  & 0 \\ 0 & 0 & 2 \end{pmatrix}        & 4. \begin{pmatrix} 1 & 0 & 1 \\ 0 & 2 & 0 \\ 0 & 0 & 3 \end{pmatrix} & \end{align*}
$$

**Answer:** Recall,
>A matrix is diagonalizable iff it’s minimal polynomial can be factored into linear factors with each root has multiplicity $1$.

We can quickly say the matrix in 2 and 4 is diagonalizable.
Also, the matrix in choice 3 is in Jordan form and not diagonal. It’s can’t be diagonalizable.

We have to do some work for 1. It’s characteristic polynomial is $(x - 1)(x-2)^2$. The choice of minimal polynomial is either $(x - 1)(x-2)$ or $(x - 1)(x-2)^2$.
$$\begin{align}&(A - I)(A-2I) \\&=\begin{pmatrix} 0 & 1 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{pmatrix} \begin{pmatrix} -1 & 1 & 0 \\ 0 & 0 & 0 \\ 0 & 0 & 0 \end{pmatrix}\\&= 0\end{align}$$
Hence minimal polynomial has desired form for digonalizability. Hence it is also diagonalizable.

Hence option **3** is correct.

****
**Question 2:** Let $A$ be an $n \times n$ matrix with real entries. Which of the following is correct?

1. If $A^2=0$, then $A$ is diagonalizable over complex numbers.
2. If $A^2=I$, then $A$ is diagonalizable over real numbers.
3. If $A^2=A$, then $A$ is diagonalizable only over complex numbers.
4. The only matrix of size $n$ satisfying the characteristic polynomial of $A$ is $A$.

**Answer:** Quickly compute the minimal polynomials for 1, 2 and 3.
1. $x^2 = 0$, Minimal polynomial is $x^2$, Hence not diagonalizable.
2. $x^2=1 \Rightarrow x^2-1 = 0 \Rightarrow (x-1)(x+1) = 0$, minimal polynomial is $(x-1)(x+1)$, Hence diagonalizable.
3. $x^2 = x \Rightarrow x^2-x = 0 \Rightarrow x(x-1) = 0$, minimal polynomial is $x(x-1)$, Hence diagonalizable.
4. As we know that all similar matrices has same characteristic polynomials, hence statement is false.

Hence **2 and 3** is correct.

****
**Question 3:** Let $A$ be a $3\times 3$ matrix with $A^3=-1$. Which of the following statements are correct?

1. $A$ has three distinct eigenvalues.
2. $A$ is diagonalizable over $\mathbb{C}$.
3. $A$ is triangularizable over $\mathbb{C}$.
4. $A$ is non singular.

**Answer:**  The minimal polynomial of the above matrix is $x^3 = 1$. Since it is a matrix of order $3$ equal to the degree of minimal polynomial, hence it is actually the characteristic polynomial. It has three distinct roots in $\mathbb{C}$, so it has three distinct eigenvalues, which also implies that it is diagonalizable.
A diagonal matrix is also triangular hence it is also triangularizable.
Characteristic polynomial has constant term hence non-singular.

Hence **all** are correct.

****
**Question 4:** A linear operator $T$ on complex vector space $V$ has characteristic polynomial $x^3(x-5)^2$ and minimal polynomials $x^2(x-5)$.Choose all correct options.

1. The Jordan form of $T$ is uniquely determined by the given information.
2. There are exactly $2$  Jordan blocks in the Jordan decomposition of $T$.
3. The operator induced by $T$ on the quotient space $V/\ker (T-5I)$ is nilpotent, where $I$ is the identity operator.
4. The operator induced by $T$ on the quotient space $V/\ker (T-5I)$ is scalar multiple of the identity operator.

**Answer:** Linear operator $T$ has two eigenvalue $\lambda = 0,5$ with multiplicity $3$ and $2$ respectively. Now look at the minimal polynomial, the eigenvalues $0, 5$ has multiplicity $2$ and $1$ respectively. Jordan block corresponding to $5$ is diagonal.
$$ J_5 =[5] \oplus [5] = \begin{pmatrix} 5 & 0 \\ 0 & 5 \end{pmatrix}$$
Now concentrate on $\lambda = 0$. It has multiplicity of $2$ in minimal polynomial hence it must have a Jordan block of order 2. But the multiplicity of $0$ in characteristic polynomial is $3$, we have one more jordan block of order $1$, hence
$$ J_0 = [0] \oplus \begin{pmatrix} 0 & 1 \\ 0 & 0 \end{pmatrix}$$
Hence it has four Jordan block and it is uniquely identified.
Hence option 1 is correct.
[yet to do some work]

******
**Question 5:** Let $N$ be a non-zero $3\times 3$ matrix with the property $N^2=0$. Which of the following is/are true?

1. $N$ is not similar to a diagonal matrix.
2. $N$ is similar to a diagonal matrix.
3. $N$ has non-zero eigenvector.
4. $N$ has three linearly independent eigenvectors.

**Answer:** The minimal polynomial is $x^2$, hence the matrix is not diagonalizable and it’s has no eigenvalue other than $0$. Also note that a matrix is diagonalizable if and only if it has $n$ linearly independent eigenvectors.

Hence only option **1** is correct.

*****
**Question 6:** Let $A=\begin{bmatrix}0 & 0 & 0 & -4 \\ 1 & 0 & 0 & 0 \\ 0 & 1 & 0 & 5 \\ 0 & 0 & 1 & 0\end{bmatrix} $. Then a Jordan canonical form of $A$ is

$$\begin{align*} &1. \begin{bmatrix}-1 & 0 & 0 & 0 \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 2 & 0 \\ 0 & 0 & 0 &-2 \end{bmatrix}             & 2. & \begin{bmatrix}-1 & 1 & 0 & 0 \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 2 & 0 \\ 0 & 0 & 0 &-2 \end{bmatrix}  &\\ & 3. \begin{bmatrix}1 & 1 & 0 & 0 \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 2 & 0 \\ 0 & 0 & 0 & -2\end{bmatrix}  & 4. &\begin{bmatrix}-1 & 1 & 0 & 0 \\ 0 & -1 & 0 & 0 \\ 0 & 0 & 2 & 0 \\ 0 & 0 & 0 &-2\end{bmatrix}   & \end{align*}$$

**Answer:** The characteristic polynomial of $A$ is
$$\begin{align*}f(x) &= \det(xI - A) \\&=\begin{vmatrix}x & 0 & 0 & 4 \\ -1 & x & 0 & 0 \\ 0 & -1 & x & -5 \\ 0 & 0 & -1 & x\end{vmatrix} \\ &= x^4 - 5x^2 +4 \\&= (x-1)(x+1)(x-2)(x+2)\end{align*}$$
Hence the matrix is diagonalizable

Hence option **1** is correct.
