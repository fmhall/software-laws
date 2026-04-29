---
title: The Ninety-Ninety Rule
slug: ninety-ninety-rule
category: Planning
level: Mid-Level
summary: The first 90% of code takes 90% of development time; the remaining 10% takes another 90%. Final phases like integration, testing, and bug fixes consume far more effort than anticipated.
source: https://lawsofsoftwareengineering.com/laws/ninety-ninety-rule
---

# The Ninety-Ninety Rule

## The Ninety-Ninety Rule

90%+90%

The first 90% of the code accounts for the first 90% of development time; the remaining 10% accounts for the other 90%.

## Takeaways

- The final parts of a project (polishing, edge cases, integration, bug fixes) often take far more effort than anticipated, often as much as the initial development.
- What looks like the "finishing touches" involves many tricky problems and unknowns.
- Reaching a "mostly done" state can create optimism, but the rule warns that "almost done" often means only halfway in terms of time.

## Overview

This rule quantifies the extent to which projects get stuck in the final phase. Often, teams make good progress at the start, building core functionality, which leads to optimism. Then integration, corner cases, performance tuning, and bug fixing consume an unexpectedly large amount of time, often equal to or greater than what has already been spent.

In practical terms, this rule advises that the last bit of a project is not a small bit. You should plan for a significant effort in finishing, polishing, and delivering.

It is also related to [Hofstadter's Law](hofstadters-law.md), as it is another way our estimates fall short. We do not realize how hard that last leg is.

## Examples

A team develops a new app. In three months, the core features are done, and they hit "90% of the functionality." Everyone expects to ship in one more month. Instead, integration testing reveals that multiple modules do not talk correctly, specific edge inputs crash the app, memory usage is too high. That final "10%" takes another three months.

When implementing a new website, you get a basic version up quickly (login, basic pages). The last bits: cross-browser fixes, responsive design adjustments, accessibility improvements, writing tests, and performance improvements seem like 10% of the work, but they take as much time as the main coding.

The rule is an important reminder: **Do not celebrate too early!**

## Origins

Credited to Tom Cargill of Bell Labs, and popularized by Jon Bentley's September 1985 "Bumper-Sticker Computer Science" column in Communications of the ACM. It was originally called the "Rule of Credibility", a name which did not stick.

It became popular in programming circles and is frequently referenced in discussions of why software is usually delivered late or why "90% done" claims can be misleading.

## The 180% Problem

The humor of this rule lies in the math: 90% + 90% = 180% of the originally estimated time. This is not a bug in the joke but a feature. It captures how badly we underestimate the tail end of projects.

As developers say, "We are 90% done… and the other 90% is still to go."
