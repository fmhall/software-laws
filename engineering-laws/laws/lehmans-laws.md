---
title: Lehman's Laws of Software Evolution
slug: lehmans-laws
category: Quality
level: Senior
summary: Software systems operating in the real world must continuously evolve to remain useful, and this evolution follows predictable patterns of increasing complexity and organizational constraints that limit development velocity.
source: https://lawsofsoftwareengineering.com/laws/lehmans-laws
---

# Lehman's Laws of Software Evolution

## Takeaways

- The first law, Continuing Change, establishes that systems lacking continuous updates become progressively less satisfactory. Successful software is never truly complete; it requires ongoing enhancements or users will migrate to alternatives.
- Accumulated changes increase system complexity over time (Law 2). Without deliberate refactoring efforts, internal disorder grows, slowing subsequent development activities.
- Development organizations face immutable constraints: team knowledge, process overhead, and coordination limitations prevent exponential acceleration of delivery.
- System quality declines perceptibly due to mounting expectations, environmental shifts, or accumulation of minor defects.

## Overview

Lehman's Laws articulate an inescapable characteristic of long-lived software systems in operational environments. Business applications, operating systems, and platforms must evolve continuously to retain relevance. Such change is neither discretionary nor cost-free.

Complexity naturally accumulates as software evolves. Each modification incrementally increases internal disorder unless deliberate counteraction occurs. This mounting complexity subsequently reduces development speed, amplifies risk, and escalates change costs. Development teams experience this as extended timelines.

Organizations encounter hard limits shaped by knowledge distribution, coordination overhead, and familiarity constraints on change absorption per release cycle. Expanding team size frequently reinforces rather than eliminates these limitations.

## Examples

A major enterprise resource planning (ERP) system deployed in 2000 illustrates these principles across 25 years. Continuous updates addressed new business rules, technology integrations, and interface modernization—necessary per Law 1. The organization observed that 2025 feature additions required longer development than 2005 equivalents, reflecting Laws 2 and 7. Periodic refactoring projects stabilized yearly output (Laws 4 and 5).

The Linux kernel exemplifies continuous evolution adapting to emerging hardware and requirements. Stagnation would render it obsolete. Expanded functionality and complexity necessitated subsystem maintainers. Conservation of familiarity manifests through limited rewrites and community-paced change management.

## Origins

Lehman formulated initial laws in 1974 through analysis of various software systems, including IBM's OS/360. Lehman and Belady examined version histories and growth metrics, establishing three foundational laws.

Subsequent refinement through the 1980s and 1990s expanded the framework: three laws initially (1974), then five, eventually reaching eight laws by the 1990s.

## The Eight Laws

The eight laws encompass: (1) Continuing Change, (2) Increasing Complexity, (3) Self-Regulation, (4) Conservation of Organizational Stability, (5) Conservation of Familiarity, (6) Continuing Growth, (7) Quality Degradation, and (8) Feedback System. These collectively characterize forces constraining real-world software evolution trajectories.

## Further Reading

- Programs, Life Cycles, and Laws of Software Evolution (Lehman & Belady's original 1980 paper)
- Laws of Software Evolution - The Nineties View (1997 update with additional research)
- The Evolution of the Laws of Software Evolution (Historical overview)
