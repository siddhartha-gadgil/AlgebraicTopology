---
layout: post
title: "fundamental group of the sphere"
date: 2014-08-27 11:03:38 +0530
comments: true
categories:
- notes
---

We now show the following.

**Theorem:** $\pi\_1(S^2)$ is trivial.

Pick a point $p\in S^2$, and observe that $S^2-\\{p\\} = \mathbb{R}^2$. Hence any pair of paths in $S^2-\\{p\\}$ are path-homotopic if and only if they have the same end-point, in particular any loop is homotopic to a constant loop. Hence the theorem follows from the following lemma.

**Lemma:** Any path $\alpha$ in $S^2$ with $\alpha(0)\neq p \neq \alpha(1)$ is path-homotopic to a path in $S^2-\\{p\\}$.

Observe that $S^2$ is the union of open sets $U$ and $V$ which are both homeomorphic to an open disc, with $p\in U$ and $p\notin V$. Using the Lesbesgue number theorem, we can decompose $[0, 1]$ into sub-intervals such that the image of each is contained in one of $U$ and $V$, and the endpoints are in $U\cap V$ (by grouping together intervals if necessary). We shall construct a homotopy that is constant on the boundary points of the sub-interval. We thus need to describe this on each sub-interval $J$. Note that no endpoint of a sub-interval equals $p$.

If $\alpha(J)\subset V$, then clearly $\alpha\vert\_J$ is disjoint from $p$. On the other hand, if $\alpha(J)\subset U$ then as $U-\\{p\\}$ is connected and there is a path in $U$ joining and two points in $U-\\{p\\}$ that is disjoint from $p$, $\alpha\vert\_J$ is path-homotopic to a path disjoint from $p$. Putting together these homotopies we get the result of the lemma, hence the theorem.

**Theorem:** $\mathbb{R^2}\neq \mathbb{R^3}$

*Proof:* Otherwise, deleting a point in each space will give homeomorphic, hence homotopy equivalent, spaces. However the resulting spaces are homotopy equivalent to the circle and the sphere respectively, and these have different fundamental groups.
