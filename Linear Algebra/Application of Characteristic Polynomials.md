---
layout: post
title: Application of Characteristic Polynomials
tags: [Determinant, Eigenvalue, Trace]
---

**Question 1:** Suppose the matrix
$$A=\begin{pmatrix} 40 & -29 & -11 \\ -18 & 30 & -12 \\ 26 & 24 & -50 \end{pmatrix} $$
has a certain complex number $\lambda \neq 0$ as an eigenvalue. Which of the following numbers must also be an eigenvalue of $A$?

1.  $\lambda +20$      2.  $\lambda -20$       3.  $20-\lambda$     4. $-20-\lambda$

**Answer:** The sum of each row of the given matrix is $0$, hence $0$ is an eigenvalue corresponds to eigenvector $(1,1,1)$.
Let $x$ be the third eigenvalue, then
$$\text{trace }A=x+\lambda +0=20 \Rightarrow x = 20-\lambda.$$

Hence **3** is correct choice.

*****
**Question 2:**  Let $A$ be a $3\times 3$ matrix with real entries such that $\det(A)=6$ and the trace of $A$ is $0$. If $\det(A+I)=0$, where $I$ denote the $3\times 3$ identity matrix, then the eigenvalues of $A$ are

1.  $-1,2,3$  2. $-1,2,-3$   3. $1,2,-3$    4. $-1,-2,3$

**Answer:** Note $\det(A+I)=0 \Rightarrow \det(A- (-1)I)= 0 $, hence $-1$ is a eigenvalue.
Assume other eigenvalues are $x$ and $y$. Since trace $A$ =$(-1 )^{n-1}$ (sum of eigenvalues) and det $A$ =  product of eigenvalues, we got following equations
$$\begin{align*} xy(-1) &= 6 \\ x + y -1 &= 0 \\ \Rightarrow x^2 - x - 6 &= 0 \quad i.e., \quad x = - 2, 3\end{align*}$$
Hence we get two possible set of eigenvalues, taking $x = -2$ we get $-1, -2 , 3$ and taking $x = 3$ we get $-1 ,3, -2$(Same)

Hence **4** is the correct choice.

*****
**Question 3:**  Let $A\in M_{10}(\mathbb{C})$, the vector space of $10\times 10$ matrices with entries in $\mathbb{C}$. Let $W_A$ be the subspace of $M_{10}(\mathbb{C})$ spanned by $\{A^n|n \geq =0\}$. Choose the correct statements.

1.  for any $A, \dim(W_A)\leq 10$
2.  for any $A, \dim(W_A)< 10$
3.  for some $A, 10<\dim(W_A)< 100$
4.  for any $A, \dim(W_A)= 100$

**Answer:** Here we use Cayley-Hamilton Theorem, which says
Every square matrix satisfies it’s characteristic polynomial. The characteristic polynomial for any square matrix of order $n$ is a monic polynomial of degree $n$.

The dimension of the matrix spanned by  $\{A^n|n \geq =0\}$ will be equal to number element linearly independent in the set. Since the matrix satisfies a monic polynomial of degree $n$, we can write $A^n$ as a linear combination of $I, A, \cdots, A^{n-1}$ as follows
$$ A^n + c_{n-1} A^{n-1} + \cdots + c_0 I = 0 \Rightarrow A^n = -c_{n-1} A^{n-1} - \cdots - c_0 I $$
Similarly all higher powers of $A^n$ can be written as linear combination of $I, A, \cdots, A^{n-1}$, hence dimension of the given set can be at most number of element in $I, A, \cdots, A^{n-1}$, $i.e.$, $10$.

Hence option **1** is correct.

*****
**Question 4:** Let $J$ denote a $101 \times 101 $ matrix with all the entries equal to $1$ and let $I$ denote the identity matrix of order $101$. Then the determinant of $J - I$ is

$1.~101 \quad  2. ~1 \quad 3. ~0  \quad 4.~100$

**Answer:** Few thing to consider
>- $\det(A) = $ product of eigenvalues of $A$.
>- If $\lambda$ an eigenvalue of any matrix $A$ then for any real number $r$, $\lambda + r$ will be the eigenvalue of matrix $A + rI$.
(Why?)  $(A+rI)v = Av + rIv = \lambda v + rv = (\lambda + r)v$

**Find all the eigenvalues of $J$:** Since $J-0I     = J$, Clearly $0$ is an eigenvalues of $J$. Multiplicity of $0$ in the characteristic polynomial is equal to $\text{nullity }(J-0I) = 101-\text{rank }(J-0I) = 101 - 1 = 100$.
Hence we get $100$ out of $101$ possible eigenvalue. Note that $(1,1,\cdots , 1)^T$ is a eigenvalue of $J$ with eigenvalue $101$.

**Now the eigenvalue of $J-I$:** We have $100$ eigenvalue $-1$ and one will be $100$. Hence,
$$\det (J-I) = (-1)^{100} \times 100 = 100.$$
Hence **4** is correct choice.
