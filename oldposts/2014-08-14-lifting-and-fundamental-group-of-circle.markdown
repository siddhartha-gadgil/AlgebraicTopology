---
layout: post
title: "Lifting and the fundamental group of the circle"
date: 2014-08-14 09:55:25 +0530
comments: true
categories:
- notes
---

So far we have not shown that any fundamental group is not trivial. We shall now show that this is the case for the circle, based on so called _lifting_ of paths and homotopies to covering spaces. This is a very elegant and important construction.

We shall throughout consider spaces $X$ and $Y$ together with a map $p: Y\to X$. The basic example is when $X = S^1$, $Y= \mathbb{R}$ and $p(t) = e^{2\pi i t}$ - the map associating to a real number $t$ the point on the circle forming an angle $2\pi t$ with the horizontal.

### Even covers

Fix $X$, $Y$ and $p$ as above. An open set $U\subset X$ is said to be evenly covered if we can express $p^{-1}(U)$ as
$$p^{-1}(U) = \coprod_{i\in I} V_i$$
so that for each $i\in I$, $V_i$ is open in $Y$ and $p\vert_{V_i}: V_i\to U$ is a homeomorphism.

It is easy to see that each open interval in the circle is evenly covered. We say that $p: Y\to X$ is a _covering map_ if each point in $X$ has an evenly covered neighbourhood. Using the word covering with its two different meanings, we can express this as saying that $X$ has an open cover $ \\{U\_\alpha\\}\_{\alpha\in A} $ consisting of evenly covered neighbourhoods. In this case we say $Y$ is a covering space (or simply a cover) of $X$.

Note that if $p$ is a covering map and $x\in X$, then $p^{-1}(x)$ is a discrete space.

### Lifting

Let $f: A \to X$ be a map. A _lift_ of $f$ is a map $F: A \to Y$ so that $f=p \circ F$. For instance, given a map to the circle, a lift is a map to the real numbers so that which lifts the point on the circle to an angle corresponding to that point. We see that for paths in the space $X$ (i.e., maps from the interval to $X$) lifts always exist and are determined by their starting points.

**Theorem: (path lifting)** Let $\alpha: [0,1] \to X$ be a path and let $y\in Y$ be such that $p(y) = \alpha(0)$. Then there is a unique path $\tilde{\alpha} :[0,1] \to Y$ such that $\alpha = p \circ \tilde\alpha$ and $\tilde{\alpha}(0) = y$.

Firstly, we see that we can subdivide the interval $[0,1]$ into $n$ equal parts so that each sub-interval has image contained in an evenly covered neighbourhood. Namely, the inverse images of evenly covered neighbourhoods under $\alpha$ form an open cover of $[0, 1]$, and the Lesbesgue number theorem implies that any sufficiently small sub-interval is contained in an open set in the cover.

Next, we construct the lift (and see uniqueness) for the union of the first $k$ sub-intervals, for $k=1$, ..., $n$. At each stage, we have an interval $[x, y]$ contained in an evenly covered neighbourhood $U$ and the lift $\tilde\alpha$ defined on a set that includes $x$ but no other point in the interval. Let $p^{-1}(U) = \coprod\_{i\in I} V\_i$, and assume $\tilde\alpha(0)\in V\_j$. Then we extend $\tilde\alpha$ by defining it on $[x, y]$ to be $\tilde\alpha(s)= (p\vert\_{V\_j})^{-1}(\alpha(s))$. It is easy to see that this is continuous, and (using connectedness) the only continuous extension of the given lift.

### Local lifting

To generalise path lifting, we observe that the proof of the second step extends to the following more general situation.

**Lemma** Let $A$ be a space, $B\subset A$, $f: A \to U$ a map to an evenly covered neighbourhood of $X$ and $F\_0: B\to Y$ a lift of $f\vert\_B$. Suppose $B$ and $A$ are both connected. Then there is a unique lift $F: A\to X$ extending $F\_0$.

We sketch the proof. Let $p^{-1}(U) = \coprod\_{i\in I} V\_i$. As $B$ is connected, $F\_0(B)$ is contained in a single component, say $V\_j$, of $p^{-1}(U)$. We define $F = (p\vert\_{V\_j})^{-1} \circ f$ to get a lift extending $F\_0$. Using the connectedness of $A$, we see that any lift extending $F\_0$ must have image in $V\_j$, and so coincides with the lift we constructed.

### Homotopy lifting

Using the more general lemma from above, we see that we can lift maps from any metric space $A$, uniquely given the lift of a point $O$, provided we can write $A$ as a union of sets $A_k$ so that, if $C_k$ denotes $A_0\cup A_1\cup A_k$, with such a decomposition chosen so that

* $A_0=\\{O\\}$.
* Each $A_k$ has diameter smaller than any specified $\epsilon>0$.
* For each $k\geq 1$, $A_k$ and $A_k\cap C_{k-1}$ are connected.

We shall use this result for the case of homotopies. We record this here.

**Theorem: (Homotopy lifting)** Let $H: [0,1] \times[0, 1] \to X$ be a path and let $y\in Y$ be such that $p(y) = H(0, 0)$. Then there is a unique homotopy $\tilde{H} : [0, 1]\times [0,1]\to Y$ such that $H = p \circ \tilde{H}$ and $\tilde{H}(0, 0) = y$.

### Fundamental group of the circle

Armed with path lifting and homotopy lifting, we can compute the fundamental group of the circle.

**Theorem:** $\pi\_1(S^1, 1) = \mathbb{Z}$

We give the main steps of the proof.

* Firstly, a map $\varphi: \pi\_1(S^1, 1)\to \mathbb{Z}$ is constructed as follows. Given a path $\alpha: [0, 1]\to S^1$ with $\alpha(0)=\alpha(1)=1$, there is a unique lift $\tilde\alpha: [0, 1]\to Y$ with $\tilde\alpha (0) = 0$. Define $\varphi([\alpha]) = \tilde\alpha(1)$, which we see is an integer as $p(\tilde\alpha(1))=1$.
* To see the above lift is well-defined, use the fact that a path-homotopy $H$ lifts to a homotopy. Further, note that the lift $\tilde{H}$ is itself a path-homotopy, as $t\mapsto \tilde{H}(0, t)$ and  $t\mapsto \tilde{H}(1, t)$ are continuous functions to the discrete set $p^{-1}(1)$. Hence the end points of lifts of path-homotopic loops are equal.
* Observe that any lift of a path $\alpha$ is obtained from any other by post-composing with a translation, and the product of lifts, if defined, is a lift. Using this we see that $\varphi$ is a homomorphism.
* By construction, we see that $\varphi$ is a surjection.
* Finally, paths in $\mathbb{R}$ with the same endpoints are path-homotopic. Using this we see that $\varphi$ is injective.
