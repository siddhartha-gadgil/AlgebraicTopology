---
layout: post
title: "brouwer's fixed point theorem"
date: 2014-08-25 09:17:29 +0530
comments: true
categories:
- notes
---

We now turn to a famous and important application.

**Brouwer's fixed point theorem:** Let $f: D^2 \to D^2$ be a map. Then there is a point $x\in D^2$ with $f(x)=x$.

This is proved using the no-retraction theorem. Namely, let $f: D^2\to D^2$ be a map, which we assume has no fixed points. Then we shall construct a retraction from the disc to the circle.

For $x\in D^2$, as $f(x)\neq x$ we have a ray $l: [0, \infty) \to \mathbb{R^2}$ given by $l\_x(t) = (1-t) f(x) + tx$. This ray begins at $f(x)$ and equals $x$ at time $1$.

Let $t\_0(x)$ be the first point on the ray of time at least one which lies on the circle. By elementary geometry this is always defined.

Let $\rho(x) = l\_x(t_o(x))$, i.e., the point on the circle where $l\_x$ hits the circle at time at least one. It is easy to see that this is continuous and a retraction, contradicting the no-retraction theorem. Thus $f$ must have a fixed point.
