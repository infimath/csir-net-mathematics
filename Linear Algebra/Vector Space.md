---
layout: post
title: Abstract Vector Space
---

**Question 1:** Let $V_1,V_2$ be subspace of a vector space $V$. Which of the following is necessarily a subspace of $V$?

1. $V_1 \cap V_2$
2. $V_1 \cup V_2$
3. $V_1+V_2=\{x+y:x \in V_1, y\in V_2 \}$.
4. $V_1\setminus V_2=\{x\in V_1 \text{ and } y  \notin V_2\}$

**Answer:** Such kind problem can solved by the methods given in text books. But in exam it is better to think as different kind of subspace of $\mathbb{R}^2$ and sometime $\mathbb{R}^3$, After little practice one can find counterexamples of wrong ones quickly.

Intersection and sum of two subspaces are vector space, but union is not a subspace when one is not contained in other. Last is certainly not a vector space because $0$ does not belong to this set.

Hence **1 and 3** are correct options.

*****
**Question 2:** For arbitary subspace $U, V$ and $W$ of a finite dimensional vector space, which of the following hold:

1. $U \cap (V + W) \subset U \cap V + U \cap W $
2. $U \cap (V + W) \supset U \cap V + U \cap W $
3. $(U \cap V) + W \subset (U +W) \cap (V + W) $
4. $(U \cap V) + W \supset (U +W) \cap (V + W) $

**Answer:** Consider three lines passing through origin with different slopes in a plane. Each form a subspace of $\mathbb{R}^2$ say $U,V$ and $W$. Intersection of any two will contain only identity.

Consider LHS of first option $V + W = \mathbb{R}^2$ taking intersection with $U$, we get $U$. While RHS of first option is $\{0\} + \{0\} = \{0\}$. Hence option 1 is wrong.

Similarly we can conclude that 4 is wrong, since RHS is whole $\mathbb{R}^2$ but LHS is only $W$.

Hence options **2 and 3** are correct.
