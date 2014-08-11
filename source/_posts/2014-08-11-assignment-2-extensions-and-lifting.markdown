---
layout: post
title: "Assignment 2 - Extensions and Lifting (due August 20, 2014)"
date: 2014-08-11 09:19:10 +0530
comments: true
categories:
- assignments
---

1. Let $A$, $X$ and $Y$ be sets and $i: A \to X$ be a function. We say that a function $f: A \to Y$ _extends_ to $F: X\to Y$ if, for all $a\in A$, $F(i(a))= f(a)$. Show that **every** function $f: A \to Y$ extends to a function $F: X\to Y$ if and only if $i$ is an injection (no continuity is assumed in this question).

2. Let $X$, $Y$ and $Z$ be topological spaces and $p: Z \to Y$ be a map (i.e., continuous function). Given a map  $f: X\to Y$, a map $F: X\to Z$ is said to be a _lift_ of $f$ if, for all $x\in X$, $p(F(x))= f(x)$.

Let $X= Y = [0,1]$, $Z = [0, 1/2] \cup [1, 3/2]$ and let $p: Z\to Y$ be such that $p(z)=z$ for $z\in [0,1/2]$ and $p(z) = z- 1/2$ for $z\in [1, 3/2]$. Show that the function $f: X\to Y$, $f: x \mapsto x$, does not have a (continuous) lift $F: X\to Z$.
