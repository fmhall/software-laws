---
name: software-laws
description: Reference guide for 56 canonical laws, principles, and heuristics of software engineering — Conway's Law, Brooks's Law, Hyrum's Law, YAGNI, DRY, SOLID, CAP theorem, and more. Triggers when discussing architectural trade-offs, team scaling, process design, code quality principles, or decision-making heuristics, to provide succinct historically-grounded guidance.
metadata:
  priority: 4
  docs:
    - "https://lawsofsoftwareengineering.com/"
  pathPatterns: []
  bashPatterns: []
  importPatterns: []
retrieval:
  aliases:
    - software laws
    - engineering principles
    - software heuristics
    - famous laws
    - programming principles
  intents:
    - apply software engineering principle
    - reference a famous law
    - architectural trade-off
    - team scaling decision
    - explain a design heuristic
  entities:
    - Conway
    - Brooks
    - Hyrum
    - YAGNI
    - DRY
    - KISS
    - SOLID
    - CAP
    - Postel
    - Murphy
    - Amdahl
    - Metcalfe
    - Pareto
    - Occam
    - Goodhart
    - Parkinson
---

# Software Laws

A curated collection of 56 established laws, principles, and heuristics that shape software engineering practice. Each law lives in its own markdown file with frontmatter (category, level, summary, source), organized to inform architectural choices, team design, quality practices, and decision-making.

## When to Apply

Reference these guidelines when:

- Making architectural or design decisions that will be hard to reverse
- Scaling a team or reorganizing around a system
- Writing or reviewing code where simplicity vs. flexibility is at stake
- Estimating, planning, or assessing why a project is late
- Weighing cognitive biases or heuristics during a technical decision
- Explaining trade-offs to collaborators with a named, well-established principle

## Categories by Priority

| Priority | Category | Focus | Count |
|----------|----------|-------|-------|
| 1 | Design | Daily coding principles | 6 |
| 2 | Architecture | System-shaping trade-offs | 10 |
| 3 | Quality | Code stewardship over time | 11 |
| 4 | Teams | Org dynamics & communication | 9 |
| 5 | Planning | Estimation & process | 6 |
| 6 | Decisions | Mental models & biases | 12 |
| 7 | Scale | Performance & network effects | 3 |

## Quick Reference

### 1. Design (6)

- `yagni` — Don't build features until you actually need them
- `dry-principle` — Every piece of knowledge has one authoritative representation
- `kiss-principle` — Keep it simple; complexity is the enemy
- `solid-principles` — Five OO design rules for maintainable classes
- `law-of-demeter` — Only talk to immediate collaborators (principle of least knowledge)
- `principle-of-least-astonishment` — Components should behave the way users expect

### 2. Architecture (10)

- `hyrums-law` — With enough users, every observable behavior becomes a contract
- `galls-law` — Complex systems that work evolved from simple systems that worked
- `law-of-leaky-abstractions` — All non-trivial abstractions eventually leak
- `teslers-law` — Complexity is conserved — you can only shift it, not remove it
- `cap-theorem` — Pick two of consistency, availability, partition tolerance
- `second-system-effect` — Second designs over-engineer everything the first one lacked
- `fallacies-of-distributed-computing` — 8 assumptions about networks that always bite you
- `law-of-unintended-consequences` — Actions in complex systems produce effects you didn't plan for
- `zawinskis-law` — Every program expands until it can read email
- `conways-law` — Systems mirror the communication structure of the organization

### 3. Quality (11)

- `boy-scout-rule` — Leave the code better than you found it
- `murphys-law` — Anything that can go wrong, will
- `postels-law` — Be conservative in what you send, liberal in what you accept
- `broken-windows-theory` — Small visible decay invites more decay
- `technical-debt` — Shortcuts accrue interest; pay them down deliberately
- `linuss-law` — Given enough eyeballs, all bugs are shallow
- `kernighans-law` — Debugging is twice as hard as writing code, so don't be too clever
- `testing-pyramid` — Many unit tests, some integration, few end-to-end
- `pesticide-paradox` — Repeated tests stop finding new bugs; evolve them
- `lehmans-laws` — Software either evolves continuously or becomes irrelevant
- `sturgeons-law` — Ninety percent of everything is crud

### 4. Teams (9)

- `brooks-law` — Adding people to a late project makes it later
- `dunbars-number` — Humans maintain stable relationships with ~150 people
- `ringelmann-effect` — Per-person productivity drops as team size grows
- `prices-law` — Half the output comes from the square root of contributors
- `putts-law` — Tech is dominated by people who understand what they do not manage and vice versa
- `peter-principle` — People rise to their level of incompetence
- `bus-factor` — How many people can be hit by a bus before the project dies
- `dilbert-principle` — Incompetent employees get promoted to management to limit their damage
- `conways-law` — (Also relevant to architecture; see above)

### 5. Planning (6)

- `premature-optimization` — Premature optimization is the root of all evil (Knuth)
- `parkinsons-law` — Work expands to fill the time available
- `ninety-ninety-rule` — The first 90% takes 90% of the time; the last 10% takes the other 90%
- `hofstadters-law` — It always takes longer than you expect, even accounting for Hofstadter's Law
- `goodharts-law` — When a measure becomes a target, it ceases to be a good measure
- `gilbs-law` — Anything you need to quantify can be measured well enough to beat not measuring at all

### 6. Decisions (12)

- `dunning-kruger-effect` — Low competence correlates with over-confidence
- `hanlons-razor` — Never attribute to malice what is explained by ignorance
- `occams-razor` — Prefer the explanation with fewer assumptions
- `sunk-cost-fallacy` — Past investment shouldn't dictate future decisions
- `map-is-not-the-territory` — Your model is not the real system
- `confirmation-bias` — You seek evidence that confirms what you already believe
- `hype-cycle-amaras-law` — We overestimate tech short-term, underestimate it long-term
- `lindy-effect` — The longer something has survived, the longer it likely will
- `first-principles-thinking` — Break problems down to fundamental truths and reason up
- `inversion` — Solve problems by thinking about what would cause failure
- `pareto-principle` — 80% of effects come from 20% of causes
- `cunninghams-law` — The fastest way to get a correct answer is to post a wrong one

### 7. Scale (3)

- `amdahls-law` — Speedup from parallelization is limited by the serial portion
- `gustafsons-law` — With larger workloads, parallelization scales better than Amdahl suggests
- `metcalfes-law` — The value of a network grows with the square of its users

## How to Use

Read individual law files for full context — takeaways, overview, examples, and origins:

```
laws/conways-law.md
laws/brooks-law.md
laws/hyrums-law.md
```

Each law file contains:

- A short summary and category in frontmatter
- A level tag (Junior / Mid-Level / Senior) where the source site provides one
- Takeaways — the actionable point
- Overview — the full principle explained
- Examples — concrete scenarios showing the law in practice
- Origins — who coined it and when
- Related notes — connections to adjacent laws, where relevant
- Source URL back to lawsofsoftwareengineering.com

## Full Index

See [README.md](README.md) for a categorized index of all 56 laws with clickable links.
