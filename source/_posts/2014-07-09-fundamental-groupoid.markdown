---
layout: post
title: "Fundamental groupoid"
date: 2014-07-09 11:23:15 +0530
comments: true
categories:
- notes
---

As mentioned earlier, in algebraic topology we associated to spaces algebraic objects. The first half of this course will be focused on one such - the _fundamental group_.

We shall first construct the so called _fundamental groupoid_, so that lemmas can be proved in the generality we need. A groupoid is like a group, except that not all pairs of elements can be multiplied. A typical example is the set of invertible linear maps between subspaces of a vector space $V$, with composition as the multiplication - this is defined in the case of the codomain of the second map coinciding with the domain of the first. There are identities corresponding to each subspace, and each element is invertible in an appropriate sense.

The construction of the fundamental groupoid is in two steps. We first define a multiplication on the space of paths of a space. We then define an equivalence relation on this space, so that the multiplication makes the quotient into a groupoid.

### Paths and Multiplication

Fix a topological space $X$. For points $a,b\in X$, let $P(X; a, b)$ be the set of paths from $a$ to $b$, i.e.,
$$P(X; a,b) = \{\alpha: [0,1] \to X : \text{$\alpha$ continuous}, \alpha(0)=a, \alpha(1) = b\}.$$

For $a, b, c\in X$, we have a multiplication from $P(a, b)\times P(b,c)\to P(a,c)$ which corresponds to a path from $a$ to $b$ followed by a path from $b$ to $c$ (precise formulas will be given in the lectures).

Let $P(X)$ be the union of the sets $P(X; a,b)$. We then get a partially defined product $*$ on this from the above products. Note that this is not associative and there are no identity elements or inverses.

### Homotopy between paths and the Groupoid structure

A crucial idea is to regard paths as equivalent if one can be deformed to the other fixing end points. This gives an equivalence relation, where the deformation is called a _path homotopy_, or simply a homotopy. Formally a path homotopy is a map $H : [0,1] \times [0,1] \to X$. For paths $\alpha$ and $\beta$, we denote path homotopy by $\alpha\sim \beta$.

Let $\pi(X)$ denote the quotient of $P(X)$ by the equivalence relation given by path homotopy, with $\pi(X, a,b)$ as obvious. Then the product on $P(X)$ induces one on $\pi(X)$. Moreover, we see that this product is associative.

Furthermore, if $e_a$ denotes the constant path at $a$, then if $\alpha$ is a path from $a$ to $b$, we have $e_a * \alpha \sim \alpha$ and $\alpha * e_b \sim \alpha$. Finally, if $\bar\alpha : t \mapsto \alpha(1-t)$, then $\alpha * \bar\alpha \sim e_a$ and $\bar\alpha * \alpha \sim e_a$. This means that $*$ makes $\pi(X)$ into a groupoid.

### Fundamental group

Now pick a basepoint $x\in X$. We define the fundamental group of $X$ with basepoint $x$ to be $\pi_1(X, x)= \pi(X; x, x)$. It is straightforward to see that the groupoid structure on $\pi(X)$ makes $\pi_1(X, x)$ into a group.

### Change of basepoint

Suppose we choose a different basepoint $x'$ for the space $X$, then if there is a path $\alpha$ from $x$ to $x'$, we see that the $\pi_1(X, x)$ and $\pi_1(X, x')$ are isomorphic. Namely, we use the groupoid multiplication to construct a function $ \beta\mapsto\alpha * \beta * \bar\alpha$ from $\pi_1(X, x')$ to $\pi_1(X, x)$. Replacing $\alpha$ by $\bar\alpha$ gives a function in the opposite direction. Finally the groupoid properties show that these are inverses of each other.
