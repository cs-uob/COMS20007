---
layout: math
title: Problems
nav_order: 2
mathjax: true
parent: Part I
---

## Decision Problems

A __decision problem__ is a specification of a computational problem whose input is a string and whose output is a decision: YES or NO.  We will usually write decision problems as follows:

PROBLEM
 * *Given*:  a string $$x$$ over some alphabet     
 * *Decide*: if $$x$$ satisfies some property $$P$$

An __instance__ of a decision problem is simply a concrete example of the Given, e.g. the particular string "hello".  A __yes instance__ of a decision problem is an instance for which the decision should be YES.  A __no instance__ is an instance for which the decision should be NO.

We will typically identify decision problems with their set of yes instances:
$$
PROBLEM = \{x | P(x) \}
$$
and this is how decision problems are typically presented in Sipser's book.

## Decidability

If there is an algorithm that solves a decision problem $$P$$, in the sense that it computes the correct decision for every possible instance (in finite time), then we say that $$P$$ is __decidable__.  Otherwise we say that $$P$$ is __undecidable__.
