---
title: Pesticide Paradox
slug: pesticide-paradox
category: Quality
level: Mid-Level
summary: Repeatedly running identical tests becomes progressively less effective at finding new bugs over time. Test suites must be continuously updated with new test cases to remain effective at detecting novel defects.
source: https://lawsofsoftwareengineering.com/laws/pesticide-paradox
---

# Pesticide Paradox

## Takeaways

- Over time, an outdated test suite will identify fewer bugs. The tests remain helpful but lose effectiveness at discovering new defects.
- This paradox highlights the importance of continuously introducing fresh test data. Testers must avoid complacency, recognizing that static test scripts alone cannot sustain effectiveness indefinitely.
- By periodically creating new tests—whether through modifying existing ones, exploring new input combinations, or investigating novel boundary cases—you "refresh the pesticide" and create opportunities to catch emerging bugs.

## Overview

The "Pesticide Paradox" draws its analogy from agriculture. When identical pesticide applications occur repeatedly, pests develop resistance to the treatment.

In software testing, initial runs of a newly created test suite often discover numerous bugs. Once those bugs are fixed, running the same unchanged tests yields diminishing returns. The software becomes "resistant" to those particular tests.

Testing processes cannot remain static. Test cases require regular maintenance. Following each release cycle, testers should evaluate which bugs reached production and strengthen the test suite accordingly.

This paradox also supports exploratory testing approaches, where testers engage with applications using varied methods across iterations, identifying issues a static regression suite would overlook. The paradox does not invalidate regression testing—old tests still catch regressions—but discovering _new_ bugs requires designing _new_ tests.

## Examples

Consider a mobile application where testers initially created comprehensive test cases for login and user profile features, identifying ten bugs that were subsequently fixed. In later releases, these test cases continued passing (no new login or profile defects). However, the application added messaging functionality with limited corresponding test coverage. Within a few releases, users reported messaging crashes that the test suite failed to detect because testing remained focused on login and profile functionality.

Once the team added messaging test cases, they began uncovering these issues before release. This cycle continues until those tests stop finding new problems, then repeats with emerging features—illustrating the core principle that stagnant testing strategies eventually fail to catch novel defects.

## Origins

Dr. Boris Beizer, a prominent software testing expert, articulated this concept. It became widely recognized as one of the "seven principles of testing" within ISTQB (International Software Testing Qualifications Board) materials.

Beizer conveyed that "every method of testing will yield a pesticide paradox, bugs adapt to tests, leaving more subtle bugs behind."

## Further Reading

- Software Testing Techniques: Boris Beizer's comprehensive book on testing techniques
- ISTQB Foundation Level Syllabus: Official ISTQB syllabus covering the seven principles of testing
- Lessons Learned in Software Testing: Practical wisdom on software testing by Kaner, Bach, and Pettichord
