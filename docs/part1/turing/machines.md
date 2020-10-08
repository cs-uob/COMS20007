---
layout: obs
title: Turing Machines
nav_order: 1
mathjax: true
parent: Turing Computability
grand_parent: Part I
---

## Turing Machines

A __Turing Machine__ is a 7-tuple $$(Q,\,\Sigma,\,\Gamma,\,\delta,\,q_0,\,q_{accept},\,q_{reject})$$, where:
* $$Q$$ is a finite set of __states__.
* $$\Sigma$$ is a finite __input alphabet__ _not_ containing the __blank symbol__ $$\sqcup$$.
* $$\Gamma$$ is a finite __tape alphabet__ where $$\Sigma \cup \{\sqcup\} \subseteq \Gamma$$.
* $$\delta : Q \times \Gamma \to Q \times \Gamma \times \{L,\,R\}$$ is the __transition function__.
* $$q_0 \in Q$$ is the __start state__.
* $$q_{accept}$$ is the __accept state__.
* $$q_{reject}$$ is the __reject state__ and $$q_{accept} \neq q_{reject}$$.

### Computation

A __configuration__ is a triple comprising two strings $$u$$, $$v$$ and a state $$q$$ that we write sequentially as $$u\:q\:v$$. The idea is that $$q$$ is the current state of the machine, $$uv$$ is the current (used) portion of the tape and the head is positioned over the first letter of $$v$$.  The tape is infinite, but $$uv$$ is a finite word: the idea is that all the rest of the tape to the right of $uv$ is filled with blanks.  For this reason, we consider configurations $$u\:q\:v$$ and $$u\:q\:v\mathord{\sqcup}$$ to be identical.  Therefore, we can always assume that $$v$$ is not empty (by adding blanks if necessary).

* The __start configuration on input__ $$v$$ has $q = q_0$, $$u = \epsilon$$ and $$v$$ being the input to the machine. 
* An __accepting configuration__ is any configuration whose state is $$q_{accept}$$.
* A __rejecting configuration__ is any configuration whose state is $$q_{reject}$$.
* Accepting and rejecting configurations are also called __halting configurations__ because the computation of the machine immediately halts (terminates) if it reaches an accepting or rejecting configuration.

We say that configuration $$C_1$$ __yields__ configuration $$C_2$$ just if the machine can move from $$C_1$$ to $$C_2$$ in a single step.  This notion is defined as follows.  Suppose $$a$$, $$b$$ and $$c$$ are letters of the tape alphabet $$\Gamma$$; $$u$$ and $$v$$ are strings in $$\Gamma^*$$, and $$q_1$$ and $$q_2$$ are states.  Suppose $$C_1$$ is a configuration of shape $$u\:q_1\:bv$$, but not a halting configuration.
* _Moving left._ When $$\delta(q_1,\,b) = (q_2,\,c,\,L)$$ the machine overwrites $$b$$ with $$c$$, transitions to state $$q_2$$ and moves the head left.  There are two subcases to consider:
  * When $u$ is empty, the machine is at the far left of the tape already and the head remains stationary.  Therefore $$C_2 = u\:q_2\:cv$$.
  * When $u$ is not empty, and is therefore of shape $$wa$$, $$C_2 = w\:q_2\:acv$$.
* _Moving right._ When $$\delta(q_1,\,b) = (q_2,\,c,\,R)$$ the machine overwrites $$b$$ with $$c$$, transitions to state $$q_2$$ and moves the head right.  Therefore $$C_2 = uc\:q_2\:v$$.

### Language

A Turing machine $$M$$ __accepts__ an input word $$v$$ just if there is a sequence of configurations $$C_1,\,C_2,\,\ldots,\,C_k$$ such that:
* $$C_1$$ is the start configuration on input $$v$$
* and, for each $$i \in \{1,\ldots,k-1\}$$, $$C_i$$ yields $$C_{i+1}$$
* and $$C_k$$ is an accepting configuration.

The __language recognised by $$M$$__ is the set $$\{w \in \Sigma^* \mid \text{$M$ accepts $w$}\}$$.

### Decider

A Turing Machine $$M$$ is said to be a __decider__ just if it halts (i.e. reaches a halting configuration) on every input.  In this case the language $$\{w \in \Sigma^* \mid \text{$M$ accepts $w$}\}$$ is said to be the language __decided__ by $$M$$.