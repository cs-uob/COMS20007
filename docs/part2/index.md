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

|---
| Week  | Lecture 1                                                                                                                    | Lecture 2                                                                                                                                                                                                | [Problem Sheet](#problem-sheets)                   | Lecture 3                                                                                                                                                                                                                              |
| :---- | :-----------                                                                                                                 | :--------                                                                                                                                                                                                | :------------                                      | :--------                                                                                                                                                                                                                              |
| 4     | **Introduction**<br/>- Part 1: [Why?][l01_1] ([notes][n01_1])                                                                | **Untyped $\lambda$-calculus**<br/>- Part 1: [$\lambda$-terms and $\beta$-reduction][l02_1] ([notes][n02_1]);<br/>- Part 2: [Live coding: $\lambda$-terms and $\beta$-reduction][l02_2] ([notes][n02_2]) | **Evaluating $\lambda$-terms**                     | **Computing with $\lambda$: CBV, CBN, Church encodings**<br/>- Part 1: [Evaluation strategies][l03_1] ([notes][n03_1]);<br/>- Part 2: [Live coding: CBV (small-step)][l03_2];<br/>- Part 3: [Church encodings][l03_3] ([notes][n03_3]) |
| 5     | Break                                                                                                                        | Break                                                                                                                                                                                                    | **Reasoning about $\lambda$-terms**                | Break                                                                                                                                                                                                                                  |
| 8     | **IMP/While** ([notes][n04])<br/>- Part 1: [Introduction and syntax][l04_1];<br/>- Part 2: [Semantics of expressions][l04_2] | **Semantics of IMP**<br/>- Part 1: [Structural Operational Semantics][l05_1] ([notes][n05_1]);<br/>- Part 2: [Natural Semantics][l05_2] ([notes][n05_2])                                                 | **Reasoning about semantics and Interpreting IMP programs**                      | **Reasoning on IMP and its semantics**<br/>- Part 1: [Structural operational semantics agree with natural semantics][l06_1] ([notes][n06_1]);<br/>- Part 2: [Natural semantics agree with structural operational semantics][l06_2] ([notes][n06_2]);<br/>- Part 3: [Why do we have both, then?][l06_3] ([notes][n06_3])
| 9 | **The Abstract Machine**<br/>- Part 1: [Interpreters vs Compilers][l07_1] ([notes][n07_1]);<br/>- Part 2: [The Abstract Machine][l07_2] ([notes][n07_2]) | **Compiling IMP programs to the Abstract Machine** | **Compiling IMP programs to the Abstract Machine** | **Reasoning about compilation** |
| 10    | **Extending IMP: Procedures**                                                               | **Extending IMP: Procedures (II)**                                                                                                                                                                       | **Compiling with procedures**                        | -
{: .v-align-top }

[l01_1]: https://web.microsoftstream.com/video/e0c39a90-ad79-4288-aa36-9a2f539f151e?channelId=029543e1-41d8-4091-b07b-af0c676c468c
[n01_1]: https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Notes%20%28Part%20II%29/Lecture1-Introduction.pdf
[l02_1]: https://web.microsoftstream.com/video/99bcfe48-1b5c-4266-ab4c-a13c23e5cd89?channelId=029543e1-41d8-4091-b07b-af0c676c468c
[n02_1]: https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Notes%20%28Part%20II%29/Lecture2-Lambda%20and%20Beta.pdf
[l02_2]: https://web.microsoftstream.com/video/3e58341a-316f-4a79-9362-191f54df2baf?channelId=029543e1-41d8-4091-b07b-af0c676c468c
[n02_2]: https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Notes%20%28Part%20II%29/Lecture2-Collected.pdf
[l03_1]: https://web.microsoftstream.com/video/f9323006-ed24-4d40-98ce-8ed64f660e4e?channelId=029543e1-41d8-4091-b07b-af0c676c468c
[n03_1]: https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Notes%20%28Part%20II%29/Lecture3-CBV-CBN-Normal.pdf
[l03_2]: https://web.microsoftstream.com/video/7a4738a6-12cc-4262-ad2b-d1ba8f84e4da?channelId=029543e1-41d8-4091-b07b-af0c676c468c
[l03_3]: https://web.microsoftstream.com/video/d0bc40e3-1491-4786-ae56-a1cfb902b07f?channelId=029543e1-41d8-4091-b07b-af0c676c468c
[n03_3]: https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Notes%20%28Part%20II%29/Lecture3-Encodings.pdf
[n04]: https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Notes%20(Part%20II)/Lecture4-IMP-Syntax-ExpressionSemantics.pdf
[l04_1]: https://web.microsoftstream.com/video/eafc7bb5-b2e1-4cf5-942a-9f878cbef323
[l04_2]: https://web.microsoftstream.com/video/eafc7bb5-b2e1-4cf5-942a-9f878cbef323
[l05_1]: https://web.microsoftstream.com/video/8a98befd-cccf-4816-b7b6-57bf5987d8e9
[n05_1]: https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Notes%20(Part%20II)/Lecture5-IMP-SOS.pdf
[l05_2]: https://web.microsoftstream.com/video/457d4cf3-e2cb-42a4-8d94-8b2d029c74d1
[n05_2]: https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Notes%20(Part%20II)/Lecture5-IMP-NS.pdf
[l06_1]: https://web.microsoftstream.com/video/4cca5147-fde4-49af-92eb-da5fb065fe4d
[n06_1]: https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Notes%20(Part%20II)/Lecture6-IMP-NS-SOS.pdf
[l06_2]: https://web.microsoftstream.com/video/2d7afe93-e1f0-472b-a2c5-792035b6a2d3
[n06_2]: https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Notes%20(Part%20II)/Lecture6-IMP-SOS-NS.pdf
[l06_3]: https://web.microsoftstream.com/video/2d7afe93-e1f0-472b-a2c5-792035b6a2d3
[n06_3]: https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Notes%20(Part%20II)/Lecture6-IMP-nt.pdf
[l07_1]: https://web.microsoftstream.com/video/4b080e06-78bb-4bda-97b0-7d0dfbb6fcf1
[n07_1]: https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Notes%20(Part%20II)/Lecture7-InterpretersVsCompilers.pdf
[l07_2]: https://web.microsoftstream.com/video/54360504-21aa-4459-980d-818924d86080
[n07_2]: https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Notes%20(Part%20II)/Lecture7-AbstractMachine.pdf

You will know enough to _start_ the problem sheet for a given Week after
listening to the first two lectures of the same Week. The problem sheet and
Lecture 3 of a given Week will often be designed to be looked at together.

## Problem Sheets
The problem sheets will appear here, along with Haskell templates, when ready.
They will also be uploaded to the Files tab of the General channel in the
[COMS20007 Team](https://teams.microsoft.com/l/team/19%3add828ce0548d42159af589fd2340ec82%40thread.tacv2/conversations?groupId=ae85fd4b-b6ac-4b6c-870d-7e4451649167&tenantId=b2e47f30-cd7d-4a4e-a5da-b18cf1a4151b).

| Week | Sheet                | Starter Code        | Sample Answers     | Sample Code         |
| :--- | :----                | :-----------        | :-------------     | :----------         |
| 4    | [Problem sheet][s01] | [Starter Code][c01] | [Solutions][ans01] | [Final Code][sol01] |
| 5    | [Problem sheet][s02] | -                   | [Solutions][ans02] | -                   |
| 8    | [Problem sheet][s03] | [Starter Code][c03] | Solutions          | Final Code          |

[s01]: https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Problems%20%28Part%20II%29/lab1-sheet.pdf
[c01]: https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Problems%20%28Part%20II%29/lab1-code.zip
[ans01]: https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Problems%20(Part%20II)/lab1-solution.pdf
[sol01]: https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Problems%20(Part%20II)/lab1-solution.zip

[s02]: https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Problems%20(Part%20II)/lab2-sheet.pdf
[ans02]: https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Problems%20(Part%20II)/lab2-solution.pdf

[s03]: https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Problems%20(Part%20II)/lab3-sheet.pdf
[c03]: https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Problems%20(Part%20II)/lab3-code.zip
[ans03]:
[sol03]:


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
put some effort into expanding it. The idea here is to use the container as a
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
| 5       | -                              |
| 8.1     | Nielsons (Ch. 1)               |
| 8.2     | Nielsons (Ch. 2.1, 2.2)        |
| 8.3     | Nielsons (Ch. 2.3)             |
| 9.1     | Nielsons (Ch. 3.1)             |
| 9.2     | Nielsons (Ch. 3.2)             |
| 9.3     | Nielsons (Ch. 3.3-3.4)         |
| 10.1    | Nielsons (Ch. 2.5)             |
| 10.2    | Nielsons (Ch. 2.5)             |
