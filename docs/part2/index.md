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

<table>
  <thead>
    <tr>
      <th style="text-align: left">Week</th>
      <th style="text-align: left">Lecture 1</th>
      <th style="text-align: left">Lecture 2</th>
      <th style="text-align: left"><a href="#problem-sheets">Problem Sheet</a></th>
      <th style="text-align: left">Lecture 3</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: left; vertical-align: top">4</td>
      <td style="text-align: left; vertical-align: top">
        <strong>Introduction</strong>
        <ul>
          <li> Part 1: <a href="https://web.microsoftstream.com/video/e0c39a90-ad79-4288-aa36-9a2f539f151e?channelId=029543e1-41d8-4091-b07b-af0c676c468c">Why?</a> (<a href="https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Notes%20%28Part%20II%29/Lecture1-Introduction.pdf">notes</a>)</li>
        </ul>
      </td>
      <td style="text-align: left; vertical-align: top">
        <strong>Untyped $\lambda$-calculus</strong>
        <ul>
          <li> Part 1: <a href="https://web.microsoftstream.com/video/99bcfe48-1b5c-4266-ab4c-a13c23e5cd89?channelId=029543e1-41d8-4091-b07b-af0c676c468c">$\lambda$-terms and $\beta$-reduction</a> (<a href="https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Notes%20%28Part%20II%29/Lecture2-Lambda%20and%20Beta.pdf">notes</a>);</li>
          <li> Part 2: <a href="https://web.microsoftstream.com/video/3e58341a-316f-4a79-9362-191f54df2baf?channelId=029543e1-41d8-4091-b07b-af0c676c468c">Live coding: $\lambda$-terms and $\beta$-reduction</a> (<a href="https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Notes%20%28Part%20II%29/Lecture2-Collected.pdf">notes</a>)</li>
        </ul>
      </td>
      <td style="text-align: left; vertical-align: top"><strong>Evaluating $\lambda$-terms</strong></td>
      <td style="text-align: left; vertical-align: top">
        <strong>Computing with $\lambda$: CBV, CBN, Church encodings</strong>
        <ul>
          <li> Part 1: <a href="https://web.microsoftstream.com/video/f9323006-ed24-4d40-98ce-8ed64f660e4e?channelId=029543e1-41d8-4091-b07b-af0c676c468c">Evaluation strategies</a> (<a href="https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Notes%20%28Part%20II%29/Lecture3-CBV-CBN-Normal.pdf">notes</a>);</li>
          <li> Part 2: <a href="https://web.microsoftstream.com/video/7a4738a6-12cc-4262-ad2b-d1ba8f84e4da?channelId=029543e1-41d8-4091-b07b-af0c676c468c">Live coding: CBV (small-step)</a>;</li>
          <li> Part 3: <a href="https://web.microsoftstream.com/video/d0bc40e3-1491-4786-ae56-a1cfb902b07f?channelId=029543e1-41d8-4091-b07b-af0c676c468c">Church encodings</a> (<a href="https://uob.sharepoint.com/teams/grp-COMS20007/Shared%20Documents/General/Notes%20%28Part%20II%29/Lecture3-Encodings.pdf">notes</a>)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align: left; vertical-align: top">5</td>
      <td style="text-align: left; vertical-align: top">Break</td>
      <td style="text-align: left; vertical-align: top">Break</td>
      <td style="text-align: left; vertical-align: top"><strong>Reasoning about $\lambda$-terms</strong></td>
      <td style="text-align: left; vertical-align: top">Break</td>
    </tr>
  </tbody>
</table>

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
| 5    |                                                                                                                                      |                                                                                                                                    |                |             |

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
