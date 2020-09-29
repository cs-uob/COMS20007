---
layout: math
title: Arithmetical Definability
mathjax: true
parent: Number Theory
nav_order: 2
---

## Arithmetical Definability

Given a formula $$A$$ with free variables, say, $$\{x_1,\ldots,x_k\}$$, an __assignment__ is a mapping $$v$$ from each $x_i$ to some natural number $$v(x_i)$$.  An assignment $$v$$ __satisfies__ a formula $$A$$ just if $$A$$ is true when replacing each free variable $x_i$ by the number $$v(x_i)$$ assigned to it.  In this case, the assignment is said to be a __satisfying assignment__ for the formula.

Two formulas $$A$$ and $$B$$ that have exactly the same satisfying assignments are said to be __equivalent__, and can be used interchangably.

This allows us to define certain concepts that are not already available in the language of arithmetic.  Let $A$ be a formula with at most two free variables $$x$$ and $$y$$.  We say that a binary relation $$R \subseteq \mathbb{N} \times \mathbb{N}$$ is __definable__ by $$A$$ just if, for all assignments $$v$$, $$R(v(x),v(y))$$ iff $$v$$ satisfies $$A$$.  We say that a relation is __arithmetical__ just if it is definable by some formula of arithmetic.  The definition extends in the obvious way to relations of any arity.

For example, the following relations are definable:

  * "$$x$$ is less than or equal to $$y$$"
     
     $$
       x \leq y := \exists z.\ x + z = y
     $$

  * "$$x$$ is (striclty) less than $$y$$"

    $$
      x < y := \exists z.\ x + z = y \wedge \neg (z = 0) 
    $$

  * "$$q$$ is the quotient and $$r$$ the remainder when dividing $$x$$ by $$y$$ using integer division"

    $$
      \mathsf{INTDIV}(x,y,q,r) := x = q * y + r \wedge r < y
    $$

  * "$$y$$ divides $$x$$"

    $$
      \mathsf{DIV}(y,x) := \exists q.\ \mathsf{INTDIV}(x,y,q,0)
    $$

  * "$$x$$ is even"

    $$
      \mathsf{EVEN}(x) := \mathsf{DIV}(2,x)
    $$

Note, defining relations in this way does not add anything to the language of arithmetic, since we just treat each left-hand-side as our own short-hand/abbreviation for the right-hand-side.