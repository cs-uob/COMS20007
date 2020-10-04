---
layout: obs
title: Theories of Arithmetic
mathjax: true
parent: Number Theory
grand_parent: Part I
nav_order: 1
---

## Theories of Arithmetic

The first-order __language of arithmetic__ is a set of words built from the following symbols:
  
  * Variables $$x,\,y,\,z,\,\ldots$$ ranging over $$\mathbb{N}$$;
  * The constant symbols $0$ and $1$;
  * Function symbols $$+$$ for addition and $$*$$ for multiplication, each of arity 2 (taking two arguments);
  * Relation symbol $$=$$;
  * Quantifiers $$\forall$$ (for all) and $$\exists$$ (exists);
  * Propositional connectives $$\vee$$ (or), $$\wedge$$ (and), $$\neg$$ (not), $$\Rightarrow$$ (implies) and $$\Leftrightarrow$$ (iff);
  * Parentheses $$($$ and $$)$$.

The words of the language are called __terms__ and __formulas__.  We will use $$s$$, $$t$$, $$u$$ and variations (e.g. $$t'$$, $$t_1$$) to stand for  terms generically.  We will use $A$, $B$, $C$ (and variations) to stand for formulas, generically.  Terms and formulas can be divided into several subcategories:

  * The __terms__ are those words built using variables, the constants, the function symbols and the parentheses.  For example, $$(1 + x) * y$$ and $$0 + (1 * x) + (y * y)$$ are terms.  Terms describe natural numbers in the sense that, if we gave particular values to the variables of the term, then it could be evaluated to a number.  Although the only constants are $$0$$ and $$1$$, we can allow ourselves to write any numeral on the understanding that it is merely an abbreviation for the corresponding summation of units, e.g. $$3 := 1 + 1 + 1$$ and $$5 := 1 + 1 + 1 + 1 + 1$$.
  * The __atomic formulas__ are equations $$s = t$$ between terms.  For example, $$x * y = 1 + (2 * z)$$ is an atomic formula.
  * The __quantifier-free formulas__ are those expressions built by combining atomic formulas using the propositional connectives and parentheses.  For example $$x = 1 + y \wedge (y = 1 \Rightarrow z = x * y)$$.
  * The __formulas__ are those expressions built by combining atomic formulas using the propositional connectives, the quantifiers and parentheses.  For example, 
  $$
    \forall x.\ (\exists q.\ x = q * 2 + 0 \wedge \neg (q = 0)) \Rightarrow  x > 1
  $$
  * The __sentences__ are those formulas without any free variables.  Intuitively, sentences can be evaluated to a truth value.  For example, $$ \forall x.\ (\exists y.\ x = 2 * y)$$ is a false sentence, $$\forall x.\ (\exists y.\ x = 2 * y) \vee (\exists y.\ x = 2 * y + 1)$$ is a true sentence, but $$\forall x.\ x = y + 3$$ is not a sentence (because $$y$$ is free).

The first-order __language of Presburger Arithmetic__ is the same as the language of number theory, except we disallow the function symbol $$*$$ for multiplication.

The __theory of True Arithmetic__ is just the set of true sentences of the language of arithmetic, we write this set $$Th(\mathbb{N},+,*)$$.  The __the theory of Presburger Arithmetic__ is the set of true sentences of the language of Presburger Arithmetic, written $$Th(\mathbb{N},+)$$.  

(For those with some background in formal logic: here "true" means "true in the standard model").
