---
layout: math
title: Part II
mathjax: true
description: "Part II: Programming Languages"
permalink: /part2/
has_children: true
has_toc: false
---

# Part II: Programming Languages
This page contains all the information specific to Part II.
1. TOC
{:toc}

## Schedule

This part will cover the semantics of programming languages in theory and in practice.
* We start by introducing the untyped lambda calculus as an alternative model of computation, exploring its (simple) abstract syntax, and defining and implementing some of its (very simple) semantics.
* We will then look towards a much more earthly imperative language—IMP—and its semantics, which we'll animate as they are, and perhaps extend.
* We will think about the logical and mathematical tools we need to reason about a language's semantics, and a program's correctness.
* We will define and animate the semantics of a small stack machine, and define a translation from IMP to its language. We will implement this translation as a compiler.

| Week  | Lecture 1    | Lecture 2                  | Problem Sheet              | Lecture 3                                            |
| :---- | :----------- | :--------                  | :------------              | :--------                                            |
| 4     | Introduction | Untyped $\lambda$-calculus | Evaluating $\lambda$-terms | Computing with $\lambda$: CBV, CBN, Church encodings |

You will know enough to _start_ the problem sheet for a given Week after
listening to the first two lectures of the same Week. The problem sheet and
Lecture 3 of a given Week will often be designed to be looked at together.

## Problem Sheets
The problem sheets will appear here, along with Haskell templates, when ready.
They will also be uploaded to the Files tab of the General channel in the
[COMS20007 Team](https://teams.microsoft.com/l/team/19%3add828ce0548d42159af589fd2340ec82%40thread.tacv2/conversations?groupId=ae85fd4b-b6ac-4b6c-870d-7e4451649167&tenantId=b2e47f30-cd7d-4a4e-a5da-b18cf1a4151b).

| Week | Sheet                                                                                                                                | Starter Code                                                                                                                       | Sample Answers | Sample Code |
| :--- | :----                                                                                                                                | :-----------                                                                                                                       | :------------- | :---------- |
| 4    | [Problem sheet](https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Problems%20%28Part%20II%29/lab1-sheet.pdf) | [Starter Code](https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Problems%20%28Part%20II%29/lab1-code.zip) | Solutions      | Final Code  |

For the programming tasks, we will assume a barebones Haskell that gives you
access to a reasonable version of Cabal.

We provide a
[Vagrantfile](https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Vagrantfile),
for use with [Vagrant](https://www.vagrantup.com) and
[VirtualBox](https://www.virtualbox.org/). The recipe uses
[ghcup](https://www.haskell.org/ghcup) to set up Haskell, Cabal, as well as
Alex and Happy, which I will sometimes use for writing lexers and parser.

We've also prepared a docker container, tested to work with both `docker` and
`podman`. You can run `docker run fdupress/coms20007lab`, with appropriate
options to mount the problem files and start the command you want. The
container uses an Alpine base image and will lack creature comforts even if you
put some effort into exanding it. The idea here is to use the container as a
thin wrapper around Haskell tools, rather than a full-blown system in which
you'll do your work.

## Materials
We will refer to the following two texts:
- Benjamin Pierce's [Types and Programming Languages](https://bris.on.worldcat.org/oclc/51958338). (We will use only Chapters 5 and 6, but Chapters 1 to 4 are a generally useful read.) We refer to this as "Pierce".
- Nielson and Nielson's [Semantics with Applications: A Formal Introduction](http://www.cs.ru.nl/~herman/onderwijs/semantics2019/wiley.pdf). (The plan calls only for Chapters 1 to 3, but we might foray into Chapters 5 and 6 if time and biology cooperate.) We refer to this as "Nielsons".

In the following table, Lectures are indexed as Week.Lecture (not part) to
avoid ambiguities in case of interruptions in the schedule.

| Lecture | Additional recommended reading |
| :------ | :----------------------------- |
| 4.1     | Pierce (Ch. 1-2)               |
| 4.2     | Pierce (Ch. 5)                 |
| 4.3     | Pierce (Ch 3, 5)               |
