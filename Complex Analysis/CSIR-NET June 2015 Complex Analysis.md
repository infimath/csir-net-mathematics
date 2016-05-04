---
layout: post
title: CSIR-NET June 2015 Complex Analysis
tags: [2015, Complex Integration, Continuity, Sequence and Series]
---

**Question 1:**
$$\int_{\vert z+1 \vert = 2}\cfrac{z^2}{4-z^2}dz=$$

1. $0$.
2. $-2\pi i$.
3. $2\pi i$.
4. $1$.

**Answer:** The curve is $\gamma: \vert z+1 \vert = 2,$ only one singularity $-2$ lies inside the closed curve.
Hence by Cauchy Integral theorem,
$$\begin{align}
\int_{\gamma}\cfrac{z^2}{4-z^2}dz
&= \int_{\gamma}\cfrac{z^2/(2-z)}{z+2}dz \\
&= 2\pi i \left( \frac{(-2)^2}{2+2} \right ) \\
&=2\pi i
\end{align}$$

Hence **3** is correct choice.

*****
**Question 2:** Let $f$ be an real valued harmonic function on $\Bbb C,$ that is $f$ satisfies the equation $\frac{\partial^2 f}{\partial x^2}+\frac{\partial^2 f}{\partial y^2}=0.$ Define the functions

$$\begin{align}
g &= \frac{\partial f}{\partial x }-i\frac{\partial f}{\partial y}\\
h &= \frac{\partial f}{\partial x }+i\frac{\partial f}{\partial y}
\end{align}$$

Then,

1. $g$ and $h$ are both holomorphic function.
2. $g$ is holomorphic, but $h$ need not be holomorphic.
3. $h$ is holomorphic, but $g$ need not be holomorphic.
4. both $g$ and $h$ are identically equals to the zero function.

**Answer:** The given real function $f$ satisfies the Laplace equation $\ne^2 f$, hence it's conjugate will make a analytic complex function.  
