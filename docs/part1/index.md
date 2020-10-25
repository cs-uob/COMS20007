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
| 1    | Introduction        | First-Order Theories of Arithmetic    | FO Arithmetic       | Automata (1)                      |
| 2    | Automata (2)        | Decidability of Presburger Arithmetic | Finite Automata     | Turing Machines (1)               | 
| 3    | Turing Machines (2) | Other Machine Models                  | Turing Machines     | The Church-Turing Thesis          |
| 9    | Undecidability      | Undecidability via Reduction          | Undecidability      | Undecidability of True Arithmetic |

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


## Materials
This site contains all the definitions and theorems that you need to be able to do the problem sheets and exam for the "Computation" part of Programming Languages and Computation. 

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
