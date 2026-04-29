---
title: SOLID Principles
slug: solid-principles
category: Design
level: Mid-Level
summary: Five foundational guidelines for object-oriented design that enhance software maintainability and scalability by addressing modularity, extensibility, and robustness.
source: https://lawsofsoftwareengineering.com/laws/solid-principles
---

# SOLID Principles

## Takeaways

- Following SOLID leads to software that is easier to extend, test, and refactor without breaking existing functionality. Each principle addresses a different aspect of good OO design.
- A class with a single responsibility (SRP) that depends on well-defined interfaces (ISP, DIP) and uses inheritance appropriately (LSP) and polymorphism for extensions (OCP) will likely be easy to maintain.
- Changes to one part of the system won't cascade into breakages elsewhere, because the code is loosely coupled and well-encapsulated.
- SOLID does not guarantee a perfect design, but it provides proven guidelines for object-oriented programming.

## Overview

The SOLID principles are five high-level guidelines for object-oriented design: **Single Responsibility** (one concern per class), **Open/Closed** (open for extension, closed for modification), **Liskov Substitution** (subclasses must be substitutable for their parent), **Interface Segregation** (no forced dependency on unused interfaces), and **Dependency Inversion** (depend on abstractions, not concretions).

When applied together, these principles produce systems that are modular, extensible, and robust under change. Code becomes easier to test, refactor, and extend without breaking existing functionality.

## Examples

For the **Single Responsibility Principle**, consider a web application managing user accounts. An anti-SRP design might have a single `UserManager` class handling validation, database operations, sending emails, and logging. A better design separates these into `UserValidator`, `UserRepository`, `EmailService`, and a `UserRegistrationService` that orchestrates them. Each class has one focus, and if the email format changes, you only touch `EmailService`.

For the **Dependency Inversion Principle**, imagine a `NotificationService` that sends alerts. Without DIP, it directly uses `EmailSender` or `SMSSender`. With DIP, you define an `INotificationChannel` interface, and all senders implement it. The service depends only on the abstraction, making it easy to add new channels or swap in test doubles.

## Origins

The five SOLID principles emerged over the years and were collected and popularized by Robert C. Martin (Uncle Bob). The acronym SOLID was coined around 2004 by Michael Feathers, who noticed the initial letters spelled out a catchy word.

Uncle Bob described SRP, OCP, LSP, ISP, and DIP in various articles from the late 1990s and early 2000s, including his "Principles of Object-Oriented Design" papers and his 2002 book Agile Software Development: Principles, Patterns, and Practices. These principles drew from earlier thinkers: OCP from Bertrand Meyer (1988), LSP from Barbara Liskov (1987), ISP from work at Xerox PARC, and DIP and SRP were Martin's formulations inspired by layering and cohesion practices.

## When SOLID Goes Too Far

It's possible to overapply the SOLID principles. Sometimes, too many small interfaces or too many abstract layers are overkill for a problem and create complexity, the so-called "AbstractFactoryFactory" problem.

When used correctly, though, these principles are genuinely helpful in managing object-oriented system complexity, which is why they've become so popular to teach.
