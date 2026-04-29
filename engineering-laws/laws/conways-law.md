---
title: Conway's Law
slug: conways-law
category: Teams
level: Senior
summary: Organizations design systems that mirror their own communication structure. Software architectures reflect how teams are organized and communicate with one another.
source: https://lawsofsoftwareengineering.com/laws/conways-law
---

# Conway's Law

"Organizations design systems that mirror their own communication structure."

## Takeaways

- The architecture of software systems often mirrors the organization's org chart or team structure.
- If your company is organized in silos, you might end up with siloed software modules that don't communicate well, reflecting those barriers.
- To achieve a desired software architecture (e.g., microservices), you might need to restructure teams accordingly, because teams build software aligned with their communication paths.
- When starting a project, realize that how you split teams or departments will likely lead to software boundaries at the same places.

## Overview

Conway's Law states that software systems reflect the communication structure of the organization that builds them. A company with separate frontend, backend, and database departments will likely produce a three-tier architecture. Small, distributed teams tend to produce modular service architectures, while large, collocated teams tend to build monoliths.

To mitigate this, teams can use the Inverse Conway Maneuver: intentionally structuring the organization to match the desired software architecture.

## Examples

- A company had separate departments for frontend, backend, and database. The software they built had a three-tier architecture, with each tier independently designed by its respective department. Integration between tiers was painful because the teams had misaligned goals.
- Amazon famously organized "two-pizza teams", each owning a specific service. Conway's Law suggests that's why Amazon's architecture is service-oriented, with clear API contracts between services.

## Origins

Melvin Conway introduced the idea in his 1967 paper "How Do Committees Invent?" After Harvard Business Review rejected it for lacking formal proof, Datamation published it in 1968.

Fred Brooks later named it "Conway's Law" in _The Mythical Man-Month_, which established the concept as foundational in software engineering.

## The Spotify Model

The Spotify Model organizes teams around features rather than technologies. Cross-functional Squads (6-12 people) own end-to-end features, grouped into Tribes by business area. Chapters and Guilds provide skill-sharing across squads. It works when it solves real coordination problems, but fails when copied blindly.
