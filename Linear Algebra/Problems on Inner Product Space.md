---
layout: post
title: Problems on Inner Product Sapce
tags: [Orthogonality]
---

**Question 1:**  Let $V$ be the inner product space consisting of linear polynomials, $p:[0,1] \rightarrow \mathbb{R} (i.e., V$ consist of polynomials $p$ of the form $p(x)=ax+b, a,b \in \mathbb{R})$, with the inner product defined by
$$\langle p,q \rangle =\int_0^1 p(x)q(x) dx \text{ for } p,q\in V.$$
An orthonormal basis of $V$ is

1.   $\{1,x\}$
2.   $\{1,x\sqrt{3} \}$
3.   $\{1,(2x-1)\sqrt{3} \}$
4.   $\{1,x-\frac{1}{2} \}$

**Answer:** To obtain an orthonormal basis form any basis the standard process to use Gram-Schmit orthogonalization.

If $\{v_1, \cdots, v_n\}$ be any basis of a vector space $V$ with some inner product $< , >$, Then we get a orthogonal basis of $V$ as follows
$$\begin{align*} w_1 &= v_1 \\ w_2 &= v_2-\frac{\langle v_1,v_2 \rangle}{\langle v_1,v_1 \rangle}v_1 \\ & \vdots \\  w_i  &= v_i-\sum_{j=1}^{i-1} \frac{\langle v_i,v_j \rangle}{\langle v_j,v_j \rangle}v_j \end{align*}$$
We still need divide each vector $w_i$ by it’s norm to get a orthonormal basis.

Taking $w_1 = 1$, then $w_2 = x - \frac{\langle 1,x \rangle}{\langle 1,1 \rangle}1$
$$\langle 1,x \rangle = \int_0^1 1 \cdot x dx = \frac{1}{2}$$
Hence we get $w_2 = x - \frac{1}{2}$, but we have to scale it’s norm to $1$.
$$\begin{align*} \Vert w_2 \Vert ^2 &= \int_0^1 \left (x-\frac{1}{2}\right )^2 dx \\ &= \int_0^1 \left (x^2-x-\frac{1}{4}\right ) dx \\ &= \left [ \frac{x^3}{3}-\frac{x^2}{2} + \frac{x}{4} \right]_0^1 \\ & = \frac{1}{12}\end{align*}$$
Hence, $w'_2 = w_2 / \Vert w_2 \Vert = (2x-1)\sqrt{3}$

Hence **3** is correct.

****
**Question 2:**  Consider $\mathbb{R}^3$ with the standard inner product. Let $W$ be the subspace of $\mathbb{R}^3$ spanned by $(1,0,-1)$. Which of the following is a basis for the orthogonal complement of $W$?

1.  $\{(1,0,1),(0,1,0)\}$
2.  $\{(1,2,1),(0,1,1)\}$
3.  $\{(2,1,2),(4,2,4)\}$
4.  $\{(2,-1,2),(1,3,1),(-1,-1,-1)\}$

**Answer:** Let’s try Gram-Schmit orthogonalization where given basis is the standard basis and new orthonormal basis start with $v_1 =(1,0,-1)$
Then
$$
\begin{align}
v_2& = (0,1,0) - \frac{\langle (1,0,-1),(0,1,0) \rangle}{\langle (1,0,-1),(1,0,-1)\rangle}(1,0,-1)\\ &= (0,1,0)
\end{align}
$$
Similarly the third will be,
$$\begin{align*}v_3   &= (0,0,1) - \frac{\langle (1,0,-1),(0,0,1) \rangle}{\langle (1,0,-1),(1,0,-1)\rangle}(1,0,-1)-\frac{\langle (0,1,0),(0,0,1) \rangle}{\langle (0,1,0),(0,1,0)\rangle}(0,1,0) \\  &= (0,0,1) + \frac{1}{2}(1,0,-1) = \frac{1}{2}(1,0,1)\end{align*}$$
Here the asks about orthogonal basis only so we can scale the vector as desired.

Hence option **1** is correct.

****
**Question 3:**  Let $u,v, w$ be vectors in an inner-product space $V$, satisfying $\|u\| = \|v \| = \|w \| =2$ and $\langle u, v \rangle = 0, \langle u, w \rangle = 1, \langle v, w \rangle = -1$. Then which of the following are true?

1.  $\|w + v - u \| = 2\sqrt{2}$
2.  $\left \{\frac{1}{2}u, \frac{1}{2}v \right \}$ forms an orthonormal basis of a two dimensional subspace of $V$
3.  $w$ and $4u - w$ are orthogonal to each other.
4. $u, v, w$ are necessarily linearly independent

**Answer:** Assume $V$ is an inner product space on $\mathbb{R}$, Consider
$$
\begin{align}
& \|w + v-u \|^2 \\
&=  \langle w + v-u \rangle \langle w + v-u \rangle \\
&= \Vert w \Vert^2 + \Vert v \Vert^2 + \Vert u \Vert^2  + 2\langle w , v  \rangle-2 \langle w , u \rangle-2 \langle  v , u \rangle \\ & = 3 \times 2^2-2-2 + 0 = 8 \\
\Rightarrow & \|w + v-u \| = 2\sqrt{2}
\end{align}
$$

Hence option 1 is correct.

Since $u$ and $v$ are orthogonal, hence $\left \{\frac{1}{2}u, \frac{1}{2}v \right \}$ forms an orthogonal basis. Hence correct.

For option $3$ consider, $\langle w, 4u-w \rangle  = 4 \langle w, u \rangle -\langle w, w \rangle  = 0$, hence correct.

Option 4, definitely false, $\langle u, w \rangle = 1, \langle v, w \rangle = -1$

Hence **1, 2 and 3** are correct.
