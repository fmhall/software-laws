---
title: Amdahl's Law
slug: amdahls-law
category: Scale
level: Senior
summary: The speedup from parallelization is limited by the fraction of work that cannot be parallelized. Sequential work sets the ceiling that no amount of parallelism can overcome.
source: https://lawsofsoftwareengineering.com/laws/amdahls-law
---

# Amdahl's Law

## Amdahl's Law

The speedup from parallelization is limited by the fraction of work that cannot be parallelized.

### Takeaways

* Sequential work sets the ceiling, and no amount of parallelism can overcome it.
* Scaling exposes bottlenecks. More resources make limits visible, not disappear.
* Fix before you scale: reduce sequential paths first. Parallelism comes second.
* It applies to people, too. Decision bottlenecks can dominate at the team scale.

### Overview

As you add CPU cores, only the parallelizable fraction of your code speeds up. The sequential fraction remains unchanged and eventually dominates total execution time. If "s" is the sequential fraction, the maximum speedup with infinite parallel resources is 1/s. So if 10% is sequential, maximum speedup is 10x. If 50% is sequential, maximum speedup is only 2x.

This applies beyond hardware. If your system has a database that can't be parallelized, adding application servers hits a wall. The same holds for organizations: if one person or committee handles all architectural decisions, adding engineers increases coordination costs without increasing throughput.

### Examples

Adding application servers doesn't help if all requests hit a single database instance. One database becomes the limit.

Another example is breaking a monolith into microservices won't improve performance if all requests ultimately serialize through a shared dependency, such as an authentication or billing service.

### Origins

Gene Amdahl, a computer architect known for his work on IBM mainframes, introduced the law in 1967 at the AFIPS Spring Joint Computer Conference.

It was originally framed around processor performance but has since proven universally applicable to systems and organizations.
