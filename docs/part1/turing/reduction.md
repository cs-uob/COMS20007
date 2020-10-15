---
layout: obs
title: Reduction
nav_order: 3
mathjax: true
parent: Turing Computability
grand_parent: Part I
---

# Reductions

Language $$A \subseteq \Sigma^*$$ is __mapping reducible__ to language $$B \subseteq \Sigma^*$$, written $$A \leq_m B$$ just if there is a computable function $$f : \Sigma^* \to \Sigma^*$$ such that, for all $w \in \Sigma^*$:

$$
  w \in A \qquad\text{iff}\qquad f(w) \in B
$$

The function $$f$$ is called the __reduction__.


__Lemma:__ If $$A \leq_m B$$ then $A^c \leq_m B^c$.



__Theorem:__ If $A \leq_m B$$ and $$B$$ is Turing-recognisible then $$A$$ is Turing-recognisible.

__Corollary:__ If $$A \leq_m B$$ and $$A$$ is not Turing-recognisible, then $$B$$ is not Turing-recognisible.

__Corollary:__ If $$A \leq_m B$$ and $$A$$ is not co-Turing-recognisible, then $$B$$ is not co-Turing-recognisible.

__Corollary:__ If $$A \leq_m B$$ and $$A$$ is not Turing-decidable, then $$B$$ is not Turing-decidable.
