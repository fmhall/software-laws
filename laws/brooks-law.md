---
title: Brooks's Law
slug: brooks-law
category: Teams
level: Mid-Level
summary: Adding more developers to a late software project typically makes it later due to training overhead and increased communication complexity. Simply increasing headcount is rarely an effective solution to project delays.
source: https://lawsofsoftwareengineering.com/laws/brooks-law
---

# Brooks's Law

Adding manpower to a late software project makes it later.

## Takeaways

- Simply throwing more developers at a project that's running behind schedule usually slows it down further initially.
- New people take time to get up to speed, consuming existing team members' time for training and coordination, which reduces overall productivity.
- Instead of hoping manpower will solve slippage, adjust the scope or timeline. Be wary of 'just hire more coders' as a solution to lateness.

## Overview

Brooks's Law challenges the belief that a software development effort is perfectly divisible among people. In reality, adding a person to a project incurs training costs and increases the number of communication paths. This can outweigh that person's contribution for a while.

If a project is already late, adding new developers can cause further delays as they learn the system and may introduce new bugs. Brooks illustrated this with an analogy about the non-linear nature of certain tasks. The law doesn't say adding people never helps, but as a response to lateness, it's usually counterproductive.

## Examples

A project is one month behind schedule, so management adds 3 new developers to a 5-person team. Over the next few weeks, progress slows. The original developers spend much of their time explaining the design and code to newcomers, and merging their work causes integration headaches. The project slips further, now two months late.

A complex bug required deep knowledge of the system. Adding more people didn't help because only the original developer understood it, and more debuggers only made things worse. Scaling a software team isn't linear. After a point, more members yield less and less output per person.

## Origins

**Frederick P. Brooks Jr.**, who managed the IBM OS/360 project, formulated this law based on painful experience. His book _The Mythical Man-Month_ (1975) explores why software projects fail and where management assumptions break down.

The book challenged the notion that "man-months" are interchangeable. Brooks demonstrated through real-world examples why the assumption that 12 programmers can accomplish in one month what one programmer does in 12 months fails in software development.

## Little's Law Makes Brooks's Law Measurable

Little's Law (L = λ × W) connects work in progress, throughput, and lead time. If your team completes 5 tasks per week with 20 in progress, average lead time is 4 weeks. Push WIP to 40 with the same throughput, and lead time doubles.

When you add people to a late project, WIP grows but throughput stays flat. Little's Law shows the result: longer lead times, not shorter ones. If you want faster delivery, reduce WIP before adding people.
