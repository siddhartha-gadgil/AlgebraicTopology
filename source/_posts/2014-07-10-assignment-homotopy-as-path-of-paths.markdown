---
layout: post
title: "Assignment 1: Homotopy as path of paths (due August 11, 2014)"
date: 2014-07-10 10:39:38 +0530
comments: true
categories: 
- assignments
---

For sets $X$ and $Y$, let $X\to Y$ denote the set of functions from $X$ to $Y$. It is clear that, for a topological space $X$ there is a bijection between $([0,1]\times [0,1] \to X$ and $[0,1] \to ([0,1] \to X)$ given by associating to $H: [0,1]\times [0,1] \to X$ the function $s\mapsto (t\mapsto H(s,t))$. In this assignment, we shall see that, if we use the appropriate topology on paths in a space $X$, i.e., maps from $[0,1]$ to $X$, this is in fact a bijection between homotopies and paths of paths. 

Given topological spaces $X$ and $Y$, the _compact open_ topology on the set $C(X, Y)$ of continuous functions from $X$ to $Y$ is the topology with sub-base constructed as follows. For $K\subset X$ compact and $U\subset Y$ open, we define $V(K, U)$ to be the set of continuous functions $f: X\to Y$ with $f(K)\subset Y$. The sets $V(K, U)$ form a sub-base for the compact-open topology.

Assume henceforth that, for spaces $X$ and $Y$, $C(X, Y)$ has the compact-open topology.

1. Assume that $X$ is a compact topological space and $Y$ is a metric space. Let $f_n: X\to Y$ be a sequence of maps and $f: X\to Y$ be a map. Show that the sequence $f_n$ converges to $f$ in the compact open topology if and only if it converges uniformly to $f$.

2. Let $X$ be a topological space. Show that a function $H: [0,1]\times [0,1] \to X$ is continuous if and only if
    * for each $s\in [0,1]$, $f_s: t\mapsto H(s, t)$ is continuous.
    * the function $s\mapsto f_s$ is a continuous function from $[0,1]$ to $C([0,1], X)$ with the compact open topology.
