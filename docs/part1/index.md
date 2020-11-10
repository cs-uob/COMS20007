---
layout: obs
title: Part I
mathjax: true
description: "Part I: Computation"
has_children: true
permalink: /part1/
---

# Part I: Computation
{: .no_toc }

This page contains all the information specific to Part I.
1. TOC
{:toc}

## Schedule

This part will follow a route from logic to computability and back again:
* We start by introducing two logical theories of arithmetic, True Arithmetic and Presburger Arithmetic.
* We will show that Presburger Arithmetic is decidable (can be solved by an algorithm), using an algorithm that represents the truth of formulas as finite automata.
* In order to show that True Arithmetic is undecidable, we propose a formal definition of algorithm: the Turing Machine.
* We will argue that Turing Machines can express any conceivable algorithm.
* We will argue that many natural and interesting problems simply cannot be solved by any Turing Machine, and therefore cannot be solved by any algorithm.
* We will argue that True Arithmetic cannot be solved by any Turing Machine and hence is undecidable.


| Week | Lecture 1           | Lecture 2                             | Problem Sheet       | Lecture 3                         | 
|:-----|:--------------------|:--------------------------------------|:--------------------|:----------------------------------|
| Week 1    | __Introduction__ <br/>[1](https://web.microsoftstream.com/video/e2f7fe6e-23dc-462f-9a5d-1a3115f3c772?channelId=029543e1-41d8-4091-b07b-af0c676c468c) Informal introduction to the themes of the unit.<br/>[2](https://web.microsoftstream.com/video/8d945dd5-1508-47b9-bad2-f8bcba4c440d?channelId=029543e1-41d8-4091-b07b-af0c676c468c) Informal introduction to the logical theories we will be studying<br/>[3](https://web.microsoftstream.com/video/170f69ba-9847-47d7-8f28-aae19d0c7edf?channelId=029543e1-41d8-4091-b07b-af0c676c468c) Prerequesites and fixing notation for strings and sets      | __First-Order Theories of Arithmetic__ <br/> [1](https://web.microsoftstream.com/video/56fe0d08-bc5b-4917-8481-5294802f0d6c?channelId=029543e1-41d8-4091-b07b-af0c676c468c) The syntax of first-order arithmetic. <br/>[2](https://web.microsoftstream.com/video/3ec7b2ea-904f-4e39-8c32-9cc268876fdb?channelId=029543e1-41d8-4091-b07b-af0c676c468c) Satisfying assignments and arithmetical definability    | __FO Arithmetic__<br/>[Problems](https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Problems%20(Part%20I)/sheet1.pdf)<br/>[Solutions](https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Solutions%20(Part%20I)/sheet1.pdf)       | __Automata (1)__  <br/>[1](https://web.microsoftstream.com/video/c7eaf9ef-a50e-4391-9521-76331607115e?channelId=029543e1-41d8-4091-b07b-af0c676c468c) Introduction to finite automata by example<br/>[2](https://web.microsoftstream.com/video/cc054bf3-967f-4a12-996a-28fc6024c5a6?channelId=029543e1-41d8-4091-b07b-af0c676c468c) How to think about the design of a finite autoamta<br/>[3](https://web.microsoftstream.com/video/0e1b4449-0c62-4575-843b-ea6766fd4815?channelId=029543e1-41d8-4091-b07b-af0c676c468c) A finite automaton that can express the addition of two natural numbers |
| Week 2    | __Automata (2)__ <br/>[1](https://web.microsoftstream.com/video/726b7fe0-3528-44a3-bef2-1a704c6ed1c1?channelId=029543e1-41d8-4091-b07b-af0c676c468c) The formal definition of (nondeterministic) finite state automata <br/>[2](https://web.microsoftstream.com/video/656944bc-917a-4168-b234-a1a84e6281d1?channelId=029543e1-41d8-4091-b07b-af0c676c468c) The product construction for finite automata  <br/>[3](https://web.microsoftstream.com/video/b0c85562-7f28-4043-ac4b-65a303f87228?channelId=029543e1-41d8-4091-b07b-af0c676c468c) Determinisation of finite automata using the powerset construction       | __Decidability of Presburger Arithmetic__ <br/>[1](https://web.microsoftstream.com/video/423d56ec-db71-413c-9265-c1fb04c4b262?channelId=029543e1-41d8-4091-b07b-af0c676c468c) Deciding Presburger Arithmetic: an overview <br/> [2](https://web.microsoftstream.com/video/5de20035-3ff2-4d3f-8c7f-441bc89f1169?channelId=029543e1-41d8-4091-b07b-af0c676c468c) Transforming the formula into a convenient shape<br/>[3](https://web.microsoftstream.com/video/8b91fe48-f074-402d-b3c6-f8a5a95f9270?channelId=029543e1-41d8-4091-b07b-af0c676c468c) Building an automaton to characterise the quantifier free body<br/>[4](https://web.microsoftstream.com/video/3f9c3760-7ddf-4b66-b3b8-4bc2ed4bc538?channelId=029543e1-41d8-4091-b07b-af0c676c468c) Extending the automaton to the quantifier prefix | __Finite Automata__<br/>[Problems](https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Problems%20(Part%20I)/sheet2.pdf)<br/>[Solutions](https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Solutions%20(Part%20I)/sheet2.pdf)    | __Turing Machines (1)__ <br/> [1](https://web.microsoftstream.com/video/bebe509d-70b6-42e3-8add-a6cdffc1908e?channelId=029543e1-41d8-4091-b07b-af0c676c468c) Towards undecidability and a definition of algorithm<br/>[2](https://web.microsoftstream.com/video/09cc82cd-0602-4777-89cb-bf07cd0dd823?channelId=029543e1-41d8-4091-b07b-af0c676c468c) Turing machines by example             | 
| Week 3    | __Turing Machines (2)__<br/>[1](https://web.microsoftstream.com/video/0cbedae3-04d8-4ce6-a0c7-e58d3845fae8?channelId=029543e1-41d8-4091-b07b-af0c676c468c) The formal definition of Turing machine<br/> [2](https://web.microsoftstream.com/video/fbca8f33-6fdb-4de6-8e0c-d79eba825afc?channelId=029543e1-41d8-4091-b07b-af0c676c468c) Definition of Turing-recognisibility and Turing-decidability | __Other Machine Models__ <br/>[1](https://web.microsoftstream.com/video/3f61434d-b7ea-48fb-a262-cf0d7392ee92?channelId=029543e1-41d8-4091-b07b-af0c676c468c) Understanding the power of Turing machines by showing that extensions or variations are equivalent <br/>[2](https://web.microsoftstream.com/video/7c23fa33-56cd-459b-af8b-8566d42737d9?channelId=029543e1-41d8-4091-b07b-af0c676c468c) Multitape Turing machines and Turing machines are equally powerful <br/>[3](https://web.microsoftstream.com/video/f135c828-b1b5-4a6a-ab08-e5be804be3f5?channelId=029543e1-41d8-4091-b07b-af0c676c468c) Enumeration machines and Turing machines are equally powerful                | __Turing Machines__<br/>[Problems](https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Problems%20(Part%20I)/sheet3.pdf)<br/>[Solutions](https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Solutions%20(Part%20I)/sheet3.pdf)     | __The Church-Turing Thesis__ <br/>[1](https://web.microsoftstream.com/video/884943ae-890a-4e8a-8e21-d72b2de185d1?channelId=029543e1-41d8-4091-b07b-af0c676c468c) Imperative programming and Turing machines are equally powerful <br/>[2](https://web.microsoftstream.com/video/8aa90b1d-b315-42f6-9aeb-c5c5a13a4070?channelId=029543e1-41d8-4091-b07b-af0c676c468c) The Church-Turing thesis         |
| Week 6    | __Undecidability__ <br/>[1](https://web.microsoftstream.com/video/cee00f05-3c33-439f-85a5-0faf0857355b?channelId=029543e1-41d8-4091-b07b-af0c676c468c) The Turing machine acceptance problem is Turing-recognisible. <br/>[2](https://web.microsoftstream.com/video/901c467c-d716-4762-bc06-6a01a13b3c66?channelId=029543e1-41d8-4091-b07b-af0c676c468c) The Turing machine acceptance problem is undecidable.<br/>[3](https://web.microsoftstream.com/video/4814851b-377b-4796-8198-58df7e0c026c?channelId=029543e1-41d8-4091-b07b-af0c676c468c) Introducing corecognisibility.  How recognisibility, corecognisibility and decidability relate to each other.   | __Undecidability via Reduction__  <br/>[1](https://web.microsoftstream.com/video/476b2f6e-b851-4710-9980-e6a1d879d5c3?channelId=029543e1-41d8-4091-b07b-af0c676c468c) Undecidability of the halting problem by reduction to the Turing machine acceptance problem. <br/>[2](https://web.microsoftstream.com/video/1acfe4aa-68e1-42ba-ba2e-acc7c73fce14?channelId=029543e1-41d8-4091-b07b-af0c676c468c) Definition of mapping reducibility and illustration of its use showing undecidability of the halting problem.<br/>[3](https://web.microsoftstream.com/video/39827e88-f22b-4fa1-ab76-2e95960bd14b?channelId=029543e1-41d8-4091-b07b-af0c676c468c) Precise relationship between mapping reducibility and (co)recognisibility.  Illustration by showing that the equivalence problem for Turing machines is neither recognisible nor corecognisible.       | __Undecidability__<br/>[Problems](https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Problems%20(Part%20I)/sheet4.pdf)      | No lecture |
| Week 7    | __Undecidability of True Arithmetic__ | __Logic and Computation__ | No sheet | No lecture |

You will know enough to attempt the problem sheet for a given Week  after listening to the first two lectures of the same week, but the corresponding lab will not actually occur until the following week.

## Problem Sheets
The problem sheets are linked here (but may not be available until the appropriate week).  Solutions will be released after the Friday lab of each week.  They can also be found under the Files tab of the General channel in the [COMS20007 Team](https://teams.microsoft.com/l/team/19%3add828ce0548d42159af589fd2340ec82%40thread.tacv2/conversations?groupId=ae85fd4b-b6ac-4b6c-870d-7e4451649167&tenantId=b2e47f30-cd7d-4a4e-a5da-b18cf1a4151b).

* [Sheet 1](https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Problems%20(Part%20I)/sheet1.pdf) ([Solutions](https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Solutions%20(Part%20I)/sheet1.pdf)) 
* [Sheet 2](https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Problems%20(Part%20I)/sheet2.pdf) ([Solutions](https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Solutions%20(Part%20I)/sheet2.pdf)) 
* [Sheet 3](https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Problems%20(Part%20I)/sheet3.pdf) ([Solutions](https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Solutions%20(Part%20I)/sheet3.pdf)) 
* [Sheet 4](https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Problems%20(Part%20I)/sheet4.pdf) ([Solutions](https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Solutions%20(Part%20I)/sheet4.pdf)) 

## Mini Project

An additional, optional activity is to complete the mini project.  The aim of the project is to implement in Haskell the algorithm described in Lecture 5 for deciding Presburger Arithmetic.  

  * [Instructions](https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Mini%20Project%20(Part%20I)/miniproj.pdf)
  * [Project Skeleton](https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Mini%20Project%20(Part%20I)/presburger.zip)

You may find the resources provided for the Part II Haskell programming useful, see [here](https://cs-uob.github.io/COMS20007/part2/#problem-sheets).


## Materials
This site contains all the definitions and theorems that you need to be able to do the problem sheets and exam for the "Computation" part of Programming Languages and Computation. 

The Onenote notebook I write on in the lectures is available [here](https://uob-my.sharepoint.com/:o:/g/personal/sr17466_bristol_ac_uk/Em80TGXrzjhKq834uuX-g3sBk9buP0nhKiY2VVnCNG1Qbg?e=efIUKX).

The textbook [Introduction to the Theory of Computation](https://ebookcentral.proquest.com/lib/bristol/detail.action?docID=5133051) by Michael Sipser is the ultimate reference for the computability theory in this part of the unit, but I have collected the formal material into this site because:
* Not everyone has a paper copy of the book and the electronic version (which everyone has access to via the library catalogue) is not easy to navigate.
* I want to talk about (and therefore display) the definitions and theorems during lectures.
* The Sipser book does not cover the logic part especially well.

You will need to refer to the textbook or take notes during lectures for discussion of examples, motivation etc.

In the following table "Sipser" refers to Introduction to the Theory of Computation, 3rd edition and "Schoening" refers to [Logic for Computer Scientists](https://link-springer-com.bris.idm.oclc.org/book/10.1007%2F978-0-8176-4763-6).  Lecture number refers to an entire lecture (of which there are three per week) and not only a part of a lecture.

| Lecture | Additional recommended reading |
|:--------|:-------------------------------|
| 1       | None                           |
| 2       | Schoening (pp 67-68)           |
| 3       | Sipser (pp 31-34, 47-52)       |
| 4       | Sipser (pp 45-46, 55-56)       |
| 5       | None                           |
| 6       | Sipser (pp 165-175)            |
| 7       | Sipser (pp 165-175)            |
| 8       | Sipser (pp 176-178, 180-182)   |
| 9       | Sipser (pp 182-187)            |
