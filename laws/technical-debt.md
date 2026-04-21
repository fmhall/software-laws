---
title: Technical Debt
slug: technical-debt
category: Quality
level: Junior
summary: Technical debt represents the accumulated complexity and shortcuts in code that slow development. Like financial debt, it requires eventual repayment through refactoring and cleanup.
source: https://lawsofsoftwareengineering.com/laws/technical-debt
---

# Technical Debt

## Takeaways

- When shortcuts are taken in code, time is borrowed from the future with immediate benefits but ongoing costs (principal plus interest).
- Unpaid technical debt accrues interest—every minute spent working around messy code, bugs, and poor design represents interest payments.
- Not all technical debt is inherently negative; it can be strategically necessary for market timing or prototyping purposes.
- Debt repayment occurs through refactoring code, adding missing tests, and improving design.

## Overview

Technical debt illustrates a core tension in software engineering: the balance between speed and quality. The concept helps both developers and non-technical stakeholders understand why completed software still requires ongoing work. Quick workarounds and postponed cleanup create short-term gains but introduce complexity that becomes increasingly costly.

Effective management requires awareness when adding temporary hacks and establishing plans to address them. Teams commonly track technical debt through comments, issue trackers, or dedicated backlogs.

When consciously managed, technical debt functions as a useful tool—deliberately accepting some messiness to meet deadlines or gather feedback, then systematically cleaning it up. Ignored debt, however, becomes progressively problematic.

## Examples

A common scenario involves skipping automated tests due to deadline pressure. The feature ships successfully (debt incurred), but subsequent changes become riskier without test coverage (interest payments). Eventually, the team must pause feature development to add tests and refactor (debt repayment).

Another example: a startup pursues rapid prototyping with hardcoded variables and duplicated code to win an initial customer. This intentional debt succeeds commercially but creates a messy codebase. Continued accumulation causes bugs and performance degradation. The team responds with a dedicated refactoring sprint to resolve the most problematic areas.

## Origins

"Technical Debt" was coined by Ward Cunningham (Agile Manifesto co-author) at OOPSLA in 1992. While working on a finance application, he used the financial metaphor to explain to management why refactoring time was necessary. Cunningham compared software development to borrowing: strategic shortcuts accelerate delivery if repaid through later cleanup.
