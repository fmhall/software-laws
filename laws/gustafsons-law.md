---
title: Gustafson's Law
slug: gustafsons-law
category: Scale
level: Senior
summary: Significant speedup in parallel processing is achievable by increasing problem size rather than keeping workload fixed. As computing resources grow, developers can solve larger problems in the same time.
source: https://lawsofsoftwareengineering.com/laws/gustafsons-law
---

# Gustafson's Law

## Gustafson's Law

"It is possible to achieve significant speedup in parallel processing by increasing the problem size."

## Takeaways

- As computing resources grow, you can compute more problems in a given time, rather than solving the same issues faster.
- It opposes the pessimism of Amdahl's Law by assuming the size of the problem to be solved will increase proportionally with computing power, so that parallel processors remain busy.
- Practically, Gustafson's Law promotes the use of more resources in computation to achieve more in terms of the scope of tasks, rather than obtaining diminishing returns.
- Software and algorithms should be designed to "scale out." As available processor cores or machines increase, the amount of work that can be done can be scaled up accordingly.

## Overview

Gustafson's Law is a principle in parallel computing that offers an optimistic view of scalability. Where Amdahl's Law assumes a fixed problem size and concludes that speedup is limited by serial work, Gustafson's Law changes the perspective.

It observes that when more processors are available, developers tend to increase the problem size to use that extra power. If you have a cluster twice as powerful, you might process twice as much data in the same time.

The parallel portion of work grows with N processors while the serial portion remains about the same, leading to "scaled speedup" that can be almost linear.

Gustafson's insight is that developers naturally use more computing power by asking bigger questions.

## Examples

In high-performance computing, climate modeling or molecular simulations routinely increase model resolution when more processors are available. A weather simulation on 1000 CPUs won't just finish 1000x faster; instead, they run a far more detailed global model in the same time, yielding a better forecast.

In big data processing, if analyzing 1 million records takes an hour on one machine, a 10-machine cluster might analyze 10 million records in an hour instead of finishing in 6 minutes.

Modern distributed systems like MapReduce and Spark encourage splitting datasets into more partitions as nodes increase, keeping all processors busy.

## Origins

Gustafson's Law was formulated by computer scientist John L. Gustafson (with Edwin Barsis) in 1988, in a paper titled "Reevaluating Amdahl's Law." Gustafson was working at Sandia National Laboratories on high-performance computing.

At that time, Amdahl's 1967 result cast doubt on massively parallel supercomputers. Gustafson observed that this held only if workload was kept constant. His 1988 argument demonstrated that by increasing problem size, a 1024-processor system could achieve near-1024x speedup on suitably scaled tasks.
