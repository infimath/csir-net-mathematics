---
layout: post
title: Question on Positive Definite Matrices
---

**Question 1:** Which of the following matrices are positive definite?
$$
\begin{align*}
&1.  \begin{pmatrix}2 & 1 \\ 1 & 2\end{pmatrix}
&2.  \begin{pmatrix}1 & 2 \\ 2 & 1\end{pmatrix}  \cr
&3.  \begin{pmatrix}\phantom{-}4 & -1 \\ -1 & \phantom{-}4\end{pmatrix}
&4.  \begin{pmatrix}0 & 4 \\ 4 & 0\end{pmatrix}
\end{align*}
$$
**Answer:** There are many ways to decide weather a symmetric matrix is positive definite or not.
>1. *Using Determinant:*  Let $\Delta_i$ be the determinant of the matrix formed by taking the entries of first $i$ rows and $i$ column.
>Then the matrix is positive definite iff $\Delta_i>0$ for all $1 \leq i \leq n$.
>2. *Using Elimination:* A square symmetric matrix is positive define iff it can be reduced to echelon form with all positive pivots without using row exchanges.
>3. *Using Eigenvalues:* A symmetric matrix is positive definite iff all its eigenvalues are strictly positive.

Now try to convert each matrix to Echelon form.

We can convert 1 and 3 to echelon form with positive pivots without interchange any rows.

While we get negative pivot in 2, hence not positive definite

We need to interchange rows in 4, hence not positive definte

Hence **1** and **3** are correct.

***
**Question 2:**  Let $a,b,c$ be the positive real numbers such that $b^2+c^2 < a< 1$. Consider the $3\times 3$ matrix
$$A=\begin{pmatrix}
1 & b & c \\
b & a & 0 \\
c & 0 & 1
\end{pmatrix} $$

1.  All the eigenvalue of $A$ are negative and real number.
2.  All the eigenvalue of $A$ are positive and real number.
3.  $A$ can have a positive as well as a negative eigenvalue.
4. Eigenvalues of $A$ can be non-real complex number.

**Answer:**  First note that the given matrix is symmetric matrix, hence all eigenvalues will be real.
Here ,
$$
\begin{align*}
\Delta_1 &= 1 >0 \\
 \Delta_2 &= \begin{vmatrix} 1 & b \cr b & a\end{vmatrix} = a-b^2 > c^2 > 0
 \end{align*}
 $$
Also,
$$
\begin{align}\Delta_3 &= \det(A) = \begin{vmatrix}1 & b & c \\ b & a & 0 \\ c & 0 & 1\end{vmatrix} \\
&= c \begin{vmatrix} b & a \cr c & 0\end{vmatrix} + 1\begin{vmatrix} 1 & b \cr b & a\end{vmatrix}
\end{align}
$$
Hence, $\Delta_3 = (a - b^2) - ac^2 = c^2 - ac^2 = c^2(1-a) >0.$

As the given matrix is a positive definite matrix all the eigenvalues will be strictly positive.

Hence **2** is correct.

******
**Question 3:** Let $a_{ij}=a_ia_j, 1 \leq i, j\leq b$, where $a_1,\cdots , a_n$ are real numbers. Let $A=(a_{ij})$ be $n\times n$ matrix. Then


1. It is possible to choose $a_1,\cdots , a_n$ so as to make the matrix $A$ non-singular.
2. Then matrix $A$ is positive definite if $(a_1,\cdots , a_n)$ is nonzero vector.
3. Then matrix $A$ is positive semi-definite if $(a_1,\cdots , a_n)$ is nonzero vector.
4. For all $(a_1,\cdots , a_n)$ zero is and eigenvalue of $A$.

**Answer:** The matrix will look like,
$$A = \begin{pmatrix}a_1^2 & a_1a_2 & a_1a_3 & \cdots &a_1a_n \\ a_2a_1 & a_2^2 & a_2a_3 & \cdots & a_2a_n \\ a_3a_1 & a_3a_2 & a_3^2 & \cdots & a_3a_n \\ \vdots & \vdots &\vdots & \ddots &\vdots \\ a_na_1 &a_na_2 & a_na_3 & \cdots & a_n^2\end{pmatrix}$$
Here,
$$
\begin{align*} \Delta_1 &= \vert a_1^2 \vert = a_1^2\\ \Delta_2 &= \begin{vmatrix} a_1^2 & a_1a_2 \\ a_2a_1 & a_2^2\end{vmatrix} = a_1a_2\begin{vmatrix} a_1 & a_2 \\ a_1 & a_2\end{vmatrix} = 0\\ &\vdots \\
\Delta_i &= 0 \text{ for all i }
\end{align*}$$

**Note 1:** Since $\det(A) = \Delta_n = 0$, hence matrix is singular for all choice of $a_i$. It also implies that $0$ is an eigenvalue of $A$.
**Note 2:** Clearly matrix is not positive definite but it is semi-definite, as the condition for semi-definite is $\Delta_i \geq 0$ for all $i$.

Hence **2** and **3** are correct.
