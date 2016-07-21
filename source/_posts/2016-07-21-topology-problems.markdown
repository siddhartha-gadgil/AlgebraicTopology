---
layout: post
title: "topological problems"
date: 2016-07-21 16:22:14 +0530
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

It is not hard to see that the first problem has a positive solution and the second a negative one - in the first case we use a convex function, while the second follows using the fact that the image of a connected set is connected. We shall return to general methods after considering some more problems.

We next describe some features of the extension problem that holds for many topological problems (we use a term from logic for this that can be safely ignored).

### First order topological problems:

* These are formulated in terms of _topological spaces_ and _continuous functions_ (which we call _maps_) : both the data and unknowns are in terms of these.
* The typical conditions are equalities between various compositions of functions.
* Conditions may also be in terms of topological properties of the spaces.

## More topological problems

### Homeomorphisms problem:
Given spaces $X$ and $Y$, are there continuous functions $f: X\to Y$ and $g: Y \to X$ with compositions the identities on $X$ and $Y$?

### Lifting problem
Given spaces $D$, $X$ and $Y$ and maps $p: Y\to X$ and $f: D\to X$, is there a function $F: D \to Y$ with $f = p\circ F$?

## Solving topological problems

As we can already see in the above examples of extension problems,  showing existence and non-existence involve very different methods. Existence is typical based on constructions, generally using geometry and point-set topology.

On the other hand, the above non-existence result could be done using point-set topology because of the special nature of the spaces - with one of them disconnected. To generalize this, we view connectivity as the $0$-dimensional case of _algebraic topology_.

### What is algebraic topology?

The idea of algebraic topology is to map a (first order) topological problem to an algebraic one, with spaces mapped to groups (or other algebraic objects) and continuous functions mapped to homomorphisms. We can generally conclude that if a topological existence problem has a solution, then so does the corresponding algebraic problem.

Often simple algebraic arguments show that there is no solution to the algebraic, hence the topological, problem. For instance, if two spaces are homeomorphic, then their associated groups are isomorphic - and hence if we obtain different groups we can conclude that the given spaces are not homeomorphic.
