---
layout: post
title: "induced homomorphisms"
date: 2014-08-21 16:10:15 +0530
comments: true
categories:
---

### Induced homomorphisms

So far we have associated the fundamental group to a based space, i.e., a space with a given based point, $(X, x\_0)$ and computed this in a few cases. We shall now associate to maps between based spaces $f: (X, x\_0)\to (Y, y\_0)$ homomorphisms. Here the map  $f: (X, x\_0)\to (Y, y\_0)$ is a map from $X$ to $Y$ with $f(x\_0) = y\_0$.

We define $f\_*: \pi\_1(X, x\_0) \to \pi\_1(Y, y\_0)$ by

$$f_*([\alpha]) = [f(\alpha)]$$

for $\alpha: [0, 1]\to X$ with $\alpha(0)=\alpha(1)=x\_0$.

It is easy to see that

* $f\_\*$ is well-defined.
* $f\_\*$ is a homomorphism.
* for an identity map $id$, $id\_\*$ is the identity homomorphism.
* $(g\circ f)\_\* = g\_\*\circ f\_\*$.

These let us translate topological problems to algebraic ones to get some nice results.

### No retraction theorem

**Theorem**: There is no map $\rho: D^2 \to S^1$ so that for all $x\in S^1$, $\rho(x)=x$.

Suppose such a map $\rho: (D^2, 1)\to (S^1, 1)$ exists, if $i: (S^1, 1)\to (D^2, 1)$ denotes the inclusion, then as $\rho\circ i$ is the identity map, it follows that
$\rho\_* \circ i\_* : \pi\_1(S^1, 1) \to \pi\_1(S^1, 1)$
is the identity. But $\pi\_1(S^1, 1) = \mathbb{Z}$, while $\pi\_1(D^2, 1)$ is trivial. The latter shows that the homomorphism $\rho\_* $ is $0$, while the former shows that the composition $\rho\_* \circ i\_* $ is a non-zero homomorphism. This gives a contradiction.
