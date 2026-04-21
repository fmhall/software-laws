---
title: Inversion
slug: inversion
category: Decisions
level: Mid-Level
summary: Solving problems by considering opposite outcomes and working backward from them. This approach helps identify risks and design robust systems by thinking about how things can fail.
source: https://lawsofsoftwareengineering.com/laws/inversion
---

# Inversion

## Takeaways

- For any goal, also ask the inverted question. If the goal is "deliver the project on time," think about "what would make us miss the deadline?" Making a list of those factors (scope creep, underestimating tasks, etc.) can help achieve goals and avoid issues.
- Use techniques like pre-mortems. Imagine your project failed, then determine what could have caused it. This critical thinking reveals risks that optimistic planning overlooks.
- In design and testing, account for edge cases and misuse scenarios. For example, ask how a malicious user could break an API. Inverting this way leads to better solutions (adding validation, rate limiting, etc.).

## Overview

The core idea is that specific insights become clear when examining a problem from the opposite angle. In software engineering, instead of designing only for the best case, deliberately design for the worst case: What if the database goes down? What if latency spikes?

By thinking about failure modes, you add features like circuit breakers, retries, or failover strategies. Inversion pairs well with First-Principles Thinking and represents a form of defensive design leading to robust outcomes by avoiding possible problems.

## Examples

**Netflix's Chaos Monkey** exemplifies this approach. Rather than only keeping systems running, Chaos Monkey randomly terminates production servers to test resilience. This enabled Netflix to build fault-tolerant services surviving server failures.

**Test-Driven Development (TDD)** applies inversion by writing failing tests first. You define failure before implementing code to pass it, forcing consideration of failure modes before development.

## Origins

Inversion traces to investor Charlie Munger's observation: "All I want to know is where I'm going to die, so I'll never go there." Munger drew inspiration from 19th-century mathematician Carl Gustav Jacobi, who solved problems through inversion, coining "Invert, always invert."

In philosophy and Stoic practice, inversion appears as premeditatio malorum (premeditation of evils)—imagining worst-case scenarios in advance for preparedness. This represents inversion applied to life philosophy.

## Further Reading

- Poor Charlie's Almanack - Charlie Munger's collection of speeches on mental models including inversion
- Antifragile - Nassim Nicholas Taleb's exploration of systems gaining from disorder and stress
