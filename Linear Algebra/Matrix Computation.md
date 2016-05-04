---
layout: post
title: Problems on Matrix Computation
tags: [Matrix]
---

**Question 1:** Let
$$S=\left \{ A:A=[a_{ij}]_{5\times 5},a_{ij}=0 \text{ or } 1 \forall i,   ,\sum_i a_{ij}=1 \forall j \text{ and } \sum_j a_{ij}=1 \forall i  \right \}.$$
Then the number of element in $S$ is

$1. ~5^2 \quad  2. ~5^5   \quad  3.~5! \quad  4.~ 55$

**Answer:** Note that, in each row exactly one of the entries can be $1$, other have to be $0$. Hence total number of matrices will be $5!$

Hence **3** is correct option.

***
**Question 2:**  Let $A,~B$ be $n \times n$  matrices such that $BA+B^2 = I - BA^2$  here $I$ is the $n\times n$ identity matrix. Which of the following is always true?
1. $A$ is nonsingular
2. $B$ is nonsingular
3. $A +B$ is nonsingular
4. $AB$ is nonsingular

**Answer:** Here
$$\begin{align}&BA+B^2 = I - BA^2 \\  \Rightarrow & BA + B^2 + BA^2 = I \\ \Rightarrow & B(A + B + A^2) = I \end{align}$$
Clearly, the matrix $B$ is always invertible.

Hence option **2** is correct.

***
**Question 3:**  Let $A$ be a $5 \times 5$ matrix with real entries such that the sum of  the entries in each row of $A$ is $1$. Then the sum of all the entries in $A^3$ is

$1.~3 \quad  2.~15  \quad   3.~5 \quad  4.~125$

**Answer:**  Note $I_3$ satisfies the condition given above. Also $I_3^3 = I_3$. Sum of all entries of $I_3$ is $5$. Since only one option is true hence option 3 is correct.
For a more rigorous proof consider the problem “If $A$ and $B$ are two square matrices such that sum of entries of each row is equal to $1$. Then the matrix $AB$ has sum of all entries in each row is $1$.”
For solution consider $C = AB$, for each $i$ we have
$$ \sum_{j = 0}^n  c_{ij} = \sum_{j = 0}^n (\sum_{k = 0}^n a_{ik}b_{kj})$$
Since the matrix has only finite number of terms, hence we can interchange the summation. $i.e.$,
$$ \sum_{j = 0}^n  c_{ij} = \sum_{k = 0}^n(\sum_{j = 0}^n a_{ik}b_{kj})$$
Note $a_{ik}$ does not depend on $j$ so we we can take it out of small bracket. $i.e.$,
$$
\begin{align*} \sum_{j = 0}^n  c_{ij} &= \sum_{k = 0}^n a_{ik} (\sum_{j = 0}^n b_{kj}) \\  & = \sum_{k = 0}^n a_{ik} \cdot 1 = 1 \end{align*}$$
Applying  this question question twice we get $A^3$ will also sum of all entries of each row equal to $1$. Since $A^3$  will be $5 \times 5$ matrix have $5$ rows. Hence $5$ is correct answer.

Hence option **3** is correct.
