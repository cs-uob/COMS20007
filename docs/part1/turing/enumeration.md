---
layout: obs
title: Enumeration Machines
nav_order: 2
mathjax: true
parent: Turing Computability
grand_parent: Part I
---

I'm not going to give a formal definition because I think the following informal description will suffice.

An __enumeration machine__ is a finite automaton equipped with two tapes.  The __work tape__ is read/write and the __output tape__ is write-only.  The machine's output tape head moves only after writing a letter to the tape, and then only by one cell to the right each time.  It may only write letters from its input alphabet to the output tape, but it may write any letter from the tape alphabet to the work tape.  There are no accept or reject states, but a distinguished __enumeration state__, which is used to signal that it has finished writing a word to the output tape.

The machine starts with both tapes blank and proceeds to transition from one configuration to the next according to its transition function.  Each step is determined by its state and the letter underneath the head of the work tape.  The actions it can perform are to overwrite the letter under the work-tape head and, optionally, to write a letter to the blank cell under the output-tape head.  It can move the work-tape head left or right by one cell.  

When the machine enters the enumeration state, the word on the output tape is considered to be __enumerated__, the contents of the output tape are erased and the output-tape head returned to the leftmost position.  The work-tape and work-tape head are unaffected.

The machine runs forever, and the language recognised by an enumeration machine $$E$$ is just the set of words that are ever enumerated by $$E$$.