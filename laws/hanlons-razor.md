---
title: Hanlon's Razor
slug: hanlons-razor
category: Decisions
level: Junior
summary: Never attribute to malice that which is adequately explained by stupidity or carelessness. When something goes wrong, assume human error or misunderstanding before suspecting intentional harm.
source: https://lawsofsoftwareengineering.com/laws/hanlons-razor
---

# Hanlon's Razor

## Hanlon's Razor

Never attribute to malice that which is adequately explained by stupidity or carelessness.

## Takeaways

* When something goes wrong, it's likely not malicious but rather an error or misunderstanding.
* Don't jump to "the system is hacked" or "someone intentionally broke this." First, consider simpler explanations (e.g., a configuration file was missed or a typographical error).
* If a colleague's code is problematic, it's probably not sabotage. It may be due to being rushed or unaware of something. Try to approach with questions, not accusations.

## Overview

Hanlon's Razor advises against assuming bad faith when an outcome may be due to human error or ignorance. If a commit introduces a security hole, it's probably a mistake, not intentional sabotage. So one responds with help and fixes, not with blame.

This doesn't mean ignoring the possibility of malice when truly warranted (security does consider malicious actors). But for day-to-day development and operations, Hanlon's Razor keeps you grounded: the build failed likely due to a misconfiguration, not because someone deliberately broke it.

## Examples

A customer reports that your software "deleted all my data!" It's easy to panic and think a disgruntled employee planted a logic bomb. But Hanlon's Razor would have you first check for a mundane bug, perhaps a boundary condition in a delete function that wipes more than intended. Indeed, you find a bug where, when a user's account name was empty, the cleanup script deleted all records. No malice, just a bug.

In security, consider a sudden spike in server traffic. Before screaming "it's a DDoS attack!", check first if it's a misconfigured client spamming or a known pattern. Most weird behaviors in systems are due to mistakes, not malicious intent.

## Origins

**Robert J. Hanlon** submitted this principle to a 1980 compilation of Murphy's Law variations. It echoes similar statements by Napoleon and Goethe about not attributing malice where incompetence can explain it.
