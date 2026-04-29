---
name: ux-laws
description: Reference guide for 30 canonical laws, principles, and effects of user experience design — Hick's Law, Fitts's Law, Jakob's Law, Miller's Law, Peak-End Rule, the Gestalt principles, and more. Triggers when discussing interface trade-offs, usability decisions, information architecture, attention and memory constraints, or persuasive design heuristics, to provide succinct evidence-grounded guidance.
metadata:
  priority: 4
  docs:
    - "https://lawsofux.com/"
retrieval:
  aliases:
    - ux laws
    - laws of ux
    - ux principles
    - usability heuristics
    - design psychology
    - cognitive principles
  intents:
    - apply a ux principle
    - reference a usability law
    - resolve a ui design trade-off
    - reduce cognitive load
    - improve information hierarchy
    - explain user behavior
  entities:
    - Fitts
    - Hick
    - Jakob
    - Miller
    - Tesler
    - Postel
    - Pareto
    - Parkinson
    - Occam
    - Doherty
    - Zeigarnik
    - Von Restorff
    - Gestalt
    - Peak-End
    - Prägnanz
---

# Laws of UX

A curated collection of 30 established laws, principles, and effects that shape user experience design. Each law lives in its own markdown file with frontmatter (category, summary, source), organized to inform interface decisions, information architecture, and decisions about attention, memory, and behavior.

## When to Apply

Reference these guidelines when:

- Designing a new interface or screen and weighing layout, hierarchy, and density
- Reducing friction in a critical user flow (signup, checkout, onboarding)
- Debating how much choice, information, or novelty to expose to users
- Reviewing visual grouping, alignment, or whitespace decisions
- Explaining why a familiar pattern beats a clever one
- Naming a usability problem with a well-established principle a teammate can search

## Categories by Priority

| Priority | Category | Focus | Count |
|----------|----------|-------|-------|
| 1 | Cognition | Mental effort, models, simplification | 7 |
| 2 | Perception | Gestalt grouping & visual organization | 5 |
| 3 | Memory | What users retain, recall, and forget | 5 |
| 4 | Attention | Focus, salience, and time constraints | 4 |
| 5 | Behavior | How users act, motivate, and persist | 5 |
| 6 | Decision-Making | Choices, biases, and prioritization | 3 |
| 7 | Aesthetics | Visual appeal and perceived usability | 1 |

## Quick Reference

### 1. Cognition (7)

- `cognitive-load` — The mental resources needed to use an interface; minimize the irrelevant kind
- `cognitive-bias` — Systematic deviations from rational judgment that shape user choices
- `chunking` — Group related items so users can process them as a single unit
- `mental-model` — Users act on what they think the system does, not what it actually does
- `jakobs-law` — Users expect your product to work like the others they already use
- `occams-razor` — Among competing designs, prefer the one with the fewest assumptions
- `teslers-law` — Every system has irreducible complexity; decide who absorbs it

### 2. Perception (5)

- `law-of-proximity` — Items placed close together are perceived as a group
- `law-of-similarity` — Items that look alike are perceived as related
- `law-of-common-region` — Elements inside a shared boundary are perceived as a group
- `law-of-uniform-connectedness` — Visually connected elements feel more related than disconnected ones
- `law-of-pragnanz` — The eye prefers the simplest interpretation of a complex form

### 3. Memory (5)

- `millers-law` — Working memory holds about 7 (±2) items
- `working-memory` — Short-term capacity is small, fragile, and easily disrupted
- `serial-position-effect` — Users remember the first and last items in a list best
- `peak-end-rule` — Experiences are judged mostly by their peak and their end
- `zeigarnik-effect` — Incomplete tasks linger in memory more than completed ones

### 4. Attention (4)

- `selective-attention` — Users only notice what's relevant to their current goal
- `von-restorff-effect` — Items that visually break the pattern are remembered
- `doherty-threshold` — Productivity soars when system response is under ~400ms
- `flow` — Users enter deep focus when challenge matches skill

### 5. Behavior (5)

- `fittss-law` — Time to hit a target depends on its distance and size
- `goal-gradient-effect` — Motivation accelerates as users get closer to a goal
- `paradox-of-the-active-user` — Users skip manuals and learn by doing
- `parkinsons-law` — Work expands to fill the time allotted; designers can shrink it
- `postels-law` — Be liberal in what you accept from users, conservative in what you produce

### 6. Decision-Making (3)

- `hicks-law` — Decision time grows with the number and complexity of choices
- `choice-overload` — Too many options reduce satisfaction and the likelihood of choosing
- `pareto-principle` — 80% of effects come from 20% of causes; focus there

### 7. Aesthetics (1)

- `aesthetic-usability-effect` — Users perceive attractive designs as more usable

## How to Use

Read individual law files for full context — takeaways, overview, and origins:

```
laws/hicks-law.md
laws/jakobs-law.md
laws/peak-end-rule.md
```

Each law file contains:

- A short summary and category in frontmatter
- The canonical quote stating the law
- Takeaways — the actionable point
- Overview — the full principle explained
- Origins — who coined it and when
- Source URL back to lawsofux.com

## Full Index

See [README.md](README.md) for a categorized index of all 30 laws with clickable links.
