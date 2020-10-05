---
layout: obs
title: Prenex Normal Form
mathjax: true
parent: Number Theory
grand_parent: Part I
nav_order: 3
---

## Prenex Normal Form

A formula $$A$$ is said to be in __prenex normal form__ just if it has the following shape:

$$
  \mathsf{Q_1}x_1.\ \mathsf{Q_2}x_2.\ \ldots \mathsf{Q_n}x_n.\ B
$$

where $$n \geq 0$$, each $$\mathsf{Q}_i$$ is a quantifier and $$B$$ is _quantifier free_.  Here, we allow $$n=0$$ to allow ourselves to say that a quantifer-free formula $$A$$ is always in prenex normal form.

__Theorem:__ Every formula of arithmetic is equivalent to a formula in prenex normal form, whose quantifier-free part only uses the propositional connectives $\wedge$ and $\vee$ and $\neg$.

Formulas of arithmetic may be converted to prenex-normal form equivalents by applying the following rules as often as possible in order to "pull out the quantifiers".  First, it is necessary to rename bound variables to ensure that no variable name is used both for the name of a free variable and simultaneously for the name of a bound variable.

$$
    \begin{array}{rcl}
      (Qx.\ A) \wedge B   & \leadsto & Qx.\ A \wedge B \\
      A \wedge (Qx.\ B)   & \leadsto & Qx.\ A \wedge B \\
      (Qx.\ A) \vee B     & \leadsto & Qx.\ A \vee B \\
      A \vee (Qx.\ B)     & \leadsto & Qx.\ A \vee B \\
      \neg (Qx.\ A)       & \leadsto & \bar{Q}x.\ \neg A \\
      A \Rightarrow B     & \leadsto & \neg A \vee B \\
      A \Leftrightarrow B & \leadsto & (A \Rightarrow B) \wedge (B \Rightarrow A) \\
    \end{array}
$$

Here $\bar{Q}$ denotes the quantifier "dual" to $Q$, i.e. $\bar{\exists} = \forall$ and $\bar{\forall} = \exists$.  This guarantees that if $A$ is a formula to which none of the above rules are applicable, then $A$ is in prenex normal form and its quantifier free part is also implication and bi-implication (iff) free.