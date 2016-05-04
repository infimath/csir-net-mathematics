---
layout: post
title: Question on Matrix of Linear Transformation
tags: [Linear Transformation, Matrix]
---

**Question 1:** Let $W$ be the vector space of all real polynomials of degree at most 3. Define $T:W \rightarrow W$ by $T(p(x))=p'(x)$ where $p'$ is the derivative of $P$. The matrix of $T$ in the basis $\{1,x,x^2,x^3\}$, considered as column vectors, is given by
$$\begin{align*}&1.\begin{pmatrix}0 & 0 & 0 & 0 \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 2 & 0 \\ 0 & 0 & 0 & 3 \end{pmatrix} &2.\begin{pmatrix}0 & 0 & 0 & 0 \\ 1 & 0 & 0 & 0 \\ 0 & 2 & 0 & 0 \\ 0 & 0 & 3 & 0 \end{pmatrix} \\ &3.  \begin{pmatrix}0 & 1& 0 & 0 \\ 0 & 0 & 2 & 0 \\ 0 & 0 & 0 & 3 \\ 0 & 0 & 0 & 0 \end{pmatrix} &4.  \begin{pmatrix}0 & 1 & 2 & 3 \\ 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 \end{pmatrix} \end{align*}$$

**Answer:**  Any ordered basis gives an correspondence between linear transformation  and matrices.

To find the matrix of linear transformation $T: V \rightarrow W$, where ordered basis of $V$ and $W$ are $(v_1, v_2, \cdots, v_n)$ and $(w_1, w_2, \cdots, w_n)$ respectively, We have to find the coefficient of $T(v_i)$ in $W$ w.r.t $(w_1, w_2, \cdots, w_n)$, and put it in $i^{th}$ column of the matrix of $T$.

Here, $T(1) = 0 = 0 \cdot 1+0 \cdot x + 0 \cdot x^2 + 0 \cdot x^3,$ hence the coefficient of $T(1)$ is $(0,0,0,0)$.

Similarly,
$T(x) = 1 = 1 \cdot 1+0 \cdot x + 0 \cdot x^2 + 0 \cdot x^3,$ hence the coefficient of $T(1)$ is $(1,0,0,0)$.

$T(x^2) = 2x = 0 \cdot 1+2 \cdot x + 0 \cdot x^2 + 0 \cdot x^3,$ hence the coefficient of $T(1)$ is $(0,2,0,0)$.

Finally,
$T(x^3) = 3x^2 = 0 \cdot 1+0 \cdot x + 3 \cdot x^2 + 0 \cdot x^3,$ hence the coefficient of $T(1)$ is $(0,0,3,0)$.
Hence,
$$ m( T ) = \begin{pmatrix}0 & 1& 0 & 0 \\ 0 & 0 & 2 & 0 \\ 0 & 0 & 0 & 3 \\ 0 & 0 & 0 & 0 \end{pmatrix}  $$

That is option **3** is correct.

****
**Question 2:**  Let $N$ be the vector space of all polynomials of degree at most 3. Define
$$ S:N \rightarrow N \text{ by } S(p(x))=p(x+1), p\in N $$
Then the matrix of $S$ in the basis $\{1,x,x^2,x^3\}$, considered as column vectors, is given by
$$\begin{align*}&1.\begin{pmatrix}1 & 0 & 0 & 0 \\ 0 & 2 & 0 & 0 \\ 0 & 0 & 3 & 0 \\ 0 & 0 & 0 & 4 \end{pmatrix} &2. \begin{pmatrix}1 & 1 & 1 & 1 \\ 0 & 1 & 2 & 3 \\ 0 & 0 & 1 & 3 \\ 0 & 0 & 0 & 1 \end{pmatrix} \\&3.  \begin{pmatrix}0 & 2 & 0 & 0 \\ 0 & 0 & 2 & 0 \\ 0 & 0 & 0 & 3 \\ 0 & 0 & 0 & 0 \end{pmatrix}  &4.  \begin{pmatrix}0 & 1 & 2 & 3 \\ 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 \end{pmatrix} \end{align*}$$

**Answer:** Proceeding same as the last problem,
$$
\begin{align}
S(p( 1 = x^0 )) &= (x+1)^{0} = 1 \\
&= 1 \cdot 1+0 \cdot x + 0 \cdot x^2 + 0 \cdot x^3,
\end{align}
$$
hence the  coefficient of $S(1)$ is $(1,0,0,0)$.

$$
\begin{align}
S(p( x^1 )) &= (x+1)^{1} = x + 1 \\
&= 1 \cdot 1+1 \cdot x + 0 \cdot x^2 + 0 \cdot x^3,
\end{align}
$$
hence the coefficient of $S(x)$ is $(1,1,0,0)$.

$$\begin{align}S(p(x^2)) &= (x+1)^2 =x^2 + 2x + 1 \\
&= 1 \cdot 1+2 \cdot x + 1 \cdot x^2 + 0 \cdot x^3,
\end{align}
$$
hence the  coefficient of $S(x^2)$ is $(1,1,0,0)$.

$$
\begin{align}
S(p(x^3)) &= (x+1)^3 = x^3 + 3x^2 + 3x + 1 \\
&= 1 \cdot 1+3 \cdot x + 3 \cdot x^2 + 1 \cdot x^3,
\end{align}
$$
hence   the coefficient of $S(x^3)$ is $(1,3,3,1)$.

Hence,
$$ m( T ) =\begin{pmatrix}1 & 1 & 1 & 1 \\ 0 & 1 & 2 & 3 \\ 0 & 0 & 1 & 3 \\ 0 & 0 & 0 & 1 \end{pmatrix}$$

Hence option **2** is correct.

*****
**Question 3:**  A linear transformation $T$ rotates each vector in $\mathbb{R}^2$ clockwise through $90^{\circ}$. The matrix $T$ ralative to the standard ordered basis $\left(\begin{bmatrix}1 \\ 0 \end{bmatrix} ,\begin{bmatrix} 0 \\ 1 \end{bmatrix} \right)$ is
$$\begin{align*} &1.\begin{bmatrix}0 & -1 \\ -1 & 0\end{bmatrix} &2.\begin{bmatrix}0 & 1 \\ -1 & 0\end{bmatrix}\\& 3.\begin{bmatrix}0 & 1 \\ 1 & 0\end{bmatrix} &4.\begin{bmatrix}0 & -1 \\ 1 & 0\end{bmatrix} \end{align*}$$

**Answer:** We need to understand the image of basis under given rotation,
![transformation of basis](https://4c430cc74fdb489bdc87fc280314be7ce9c05b71.googledrive.com/host/0B_xlLCDkRnz2WTBKdjhfZmlSZ2s/rotation%5B7%5D.png)
$$
\begin{align}
&T(e_1) &=&-e_2 &=& 0 \cdot e_1 + (-1) \cdot e_2 \\
&T(e_2) &=& e_1 &=& 1 \cdot e_1 + 0 \cdot e_2
\end{align}
$$
Hence,
$$m( T ) = \begin{bmatrix}0 & 1 \\ -1 & 0\end{bmatrix} $$

Hence option **2** is correct.

****
**Question 4:**  For a positive integer $n$, let $P_n$ denote the space of all polynimials $p(x)$ with coefficients in $\mathbb{R}$ such that $\deg p(x) \leq n$, and let $B_n$ denote the standard basis of $P_n$ given by $B_n=\{1,x,x^2,\cdots , x^n\}$. If $T:P_3 \rightarrow P_4$ is the linear transformation defined by $T(p(x))=x^2p'(x) + \int_0^x p(t)dt$ and $A=(a_{ij})$ is the $5\times 4$ matrix of $T$ with respect of standard bases $B_3$ and $B_4$, then

1. $a_{32}=\frac{3}{2},a_{33}=\frac{7}{3}$.
2. $a_{32}=\frac{3}{2},a_{33}=0$.
3. $a_{32}=0,a_{33}=\frac{7}{3}$.
4. $a_{32}=0,a_{33}=0$.

**Answer:** Here
$T(1) = x = 0 \cdot 1+1 \cdot x + 0 \cdot x^2 + 0 \cdot x^3,$ hence the coefficient of $T(1)$ is $(0,1,0,0,0)$.
$T(x) = \frac{3}{2}x^2 = 0 \cdot 1+0 \cdot x + \frac{3}{2} \cdot x^2 + 0 \cdot x^3,$ hence the coefficient of $T(1)$ is $(0,0,\frac{3}{2},0,0)$.
$T(x^2) = \frac{5}{3}x^3 = 0 \cdot 1+0 \cdot x + 0 \cdot x^2 + 0 \frac{5}{3} x^3,$ hence the coefficient of $T(1)$ is $(0,0,0,\frac{5}{3},0)$.
$T(x^3) = \frac{13}{4}x^4 = 0 \cdot 1+0 \cdot x + 0 \cdot x^2 + \frac{13}{4} \cdot x^3,$ hence the coefficient of $T(1)$ is $(0,0,0,0,\frac{13}{4})$.
The matrix of linear transformation is
$$m( T ) = \begin{pmatrix}  0 & 0 & 0 & 0  \\ 1 & 0 & 0 & 0  \\ 0 & \frac{3}{2} & 0 & 0 \\ 0 & 0 & \frac{5}{3} & 0  \\ 0 & 0 & 0 & \frac{13}{4} \end{pmatrix}$$
Hence option **2** is correct.

****
**Question 5:**  Let $n$ be a positive integer and $V$ be an $(n+1)$ dimensional vector space over $\mathbb{R}$. If $\{e_1,e_2,\cdots,e_{n+1}\}$ is a basis of $V$ and $T:V\rightarrow V$ is the linear transformation satisfying
$$T(e_i)=e_{i+1} \text{ for } i=1,2,\cdots, n \text{ and } T(e_{n+1})=0.$$
Then

1. trace of $T$ is nonzero.
2. rank of $T$ is $n$.
3. nullity of $T$ is $1$.
4. $T^n=T\circ T \circ \cdots \circ T \text{  (n-times) is the zero map.}$

**Answer:** The matrix of linear transformation is
$$
\begin{align}
m( T ) &= \begin{pmatrix}  0 & 0 & 0&  \cdots & 0  \\ 1 & 0 & 0 &\cdots & 0 \\ 0 & 1 & 0&  \cdots & 0 \\ 0 & 0 & 1&  \cdots & 0 \\ \vdots & \vdots & \vdots &  \ddots & \vdots \\ 0 & 0 & 0&  \cdots & 0 \end{pmatrix} \\&= \begin{pmatrix} 0 & 0 \\ I_n & 0 \end{pmatrix}
\end{align}
$$
This is a matrix whose all entries are zero, except below the diagonals. It’s rank is $n$ hence nullity will be $1$. Since the above matrix is a nilpotent matrix of order $n$, hence option 4 is also true.

Combining all, **3 and 4** are correct options.
