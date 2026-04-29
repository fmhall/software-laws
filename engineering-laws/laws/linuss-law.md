---
title: Linus's Law
slug: linuss-law
category: Quality
level: Mid-Level
summary: Given enough eyeballs, all bugs are shallow. This principle demonstrates how transparency and community collaboration in open-source development lead to faster bug identification and more robust software.
source: https://lawsofsoftwareengineering.com/laws/linuss-law
---

# Linus's Law

## Takeaways

- Linus's Law highlights the strength of peer review and community in software development. If a codebase is accessible to many developers, someone will eventually have the expertise to identify and fix a given bug.
- The rule is often cited as a key advantage of open-source software. When source code is widely available, you accumulate a large pool of contributors.
- Linus's Law assumes those eyeballs are indeed looking, i.e., an active community. Simply being open-source doesn't magically fix bugs.

## Overview

Linux's open development model, releasing code early and often to the public, results in rapid bug-finding. When many people use and review a piece of software, problems become apparent to someone.

What is a perplexing bug to you might be trivial to another programmer who spots it. Or among thousands of users, one will stumble on the exact reproduction steps, and another might submit a fix.

This law shows the core of open-source: that transparency and collaboration lead to more robust, reliable software.

However, it's not absolute. Coordination and quality control are still needed. But as a guiding principle, Linus's Law captures the self-correcting nature of a large developer ecosystem.

The "many eyeballs" principle is also why internal code reviews and pair programming can be effective.

## Examples

Consider the Apache HTTP Server, an open-source web server used by millions. Because its code is open and it has a vast user base, many developers have at some point debugged or improved it. If there's a security flaw or bug, odds are high that someone in the global community will discover it and report it. The infamous "Log4Shell" vulnerability in the Log4j library was identified and patched by the community.

In contrast, consider an enterprise software product that is proprietary with only a few clients. If a subtle bug appears, only the vendor's small team and a few client implementers are likely to notice it. It might take a long time to surface and debug because of limited "eyeballs."

## Origins

The law is named after Linus Torvalds, the creator of Linux, but Eric S. Raymond formulated it in the late 1990s. In "The Cathedral and the Bazaar", Raymond captured this concept and named it in honor of Torvalds' open development approach.

The idea was inspired by the Linux community, where hundreds of developers worldwide were debugging the kernel simultaneously. The essay was first presented in 1997 and published as a book in 1999.

## The Heartbleed Counterexample

Although Linus's Law is correct, it was shown to be imperfect in 2014 when the Heartbleed bug was discovered in OpenSSL. In this instance, because OpenSSL is open source, it had been overlooked for two years. In this scenario, having many eyeballs was ineffective because no one was watching.
