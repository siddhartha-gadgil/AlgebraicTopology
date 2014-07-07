---
layout: post
title: "topology problems"
date: 2014-07-06 16:22:14 +0530
comments: true
categories: 
- notes
---

We begin with a typical topology problem (or rather, collection of problems).

###Extension problems:
Assume we are given topological spaces $X$ and $Y$, a subspace $A\subset X$ and a continuous function $f: A\to Y$. Is there an extension of $f$ to $F: X\to Y$, i.e.,  if $i:A\to X$ is the inclusion function, is there a function $F: X\to Y$ so that $f = F\circ i$?

Two specific instances of this:

1. $X = [-1,1]$, $A = \\{-1,1\\}$, $Y =\mathbb{R}$, $f: A\to Y$ is given by $f(x)= x$, for $x=-1,1$.

2. $X = [-1,1]$, $A = \\{-1,1\\}$, $Y =\mathbb{R} \setminus \{0\}$, $f: A\to Y$ is given by $f(x)= x$, for $x=-1,1$.

It is not hard to see that the first problem has a positive solution and the second a negative one. We shall return to these. But first we describe some features of the extension problem that holds for many topological problems.

### First order topological problems:

* These are formulated in terms of _topological spaces_ and _continuous functions_ (which we call _maps_) : both the data and unknowns are in terms of these. 
* The typical conditions are equalities between various compositions of functions.
* Conditions may also be in terms of topological properties of the spaces.


