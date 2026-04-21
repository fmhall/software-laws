---
title: Gilb's Law
slug: gilbs-law
category: Planning
level: Mid-Level
summary: Anything you need to quantify can be measured in some way better than not measuring it. Even approximate or indirect measurements provide valuable insight and starting points for improvement.
source: https://lawsofsoftwareengineering.com/laws/gilbs-law
---

# Gilb's Law

## Takeaways

* It is better to have some data or metric on a phenomenon than to be completely blind, as long as you understand the metric's limitations.
* In contrast to Goodhart's Law, which warns about misuse of metrics, Gilb's Law reminds us not to throw out metrics entirely.
* Start with a basic measure and refine it over time. The act of measuring helps teams focus and identify trends.
* Even an approximate or indirect measurement is better than none.

## Overview

Gilb's Law responds to the paralysis that Goodhart's Law can cause. This law asserts that even an approximate or indirect measurement is better than none. When something is essential (performance, customer satisfaction, code maintainability), you should attempt to measure it, because otherwise you have no objective feedback.

Gilb's Law is a good reply to the statement "this aspect is unmeasurable so we won't try." For example, measuring "code quality" is difficult, but you can measure indicators such as cyclomatic complexity, lint warnings, or defect rates as partial indicators. More such indicators can paint the bigger picture.

Those metrics won't be perfect, but Gilb's Law suggests that having them gives you some insight and a starting point for improvement, which is better than having no clue at all.

## Examples

Measuring **developer productivity** is notoriously hard (lines of code are poor proxies, story points can be inconsistent). However, you might use deployment frequency or change lead time (as in the DORA metrics for DevOps) as a proxy. They do not capture everything, but they give you actionable data. If deployment frequency decreases, something might be wrong with the pipeline.

Another example is **tracking Tech Debt**. No perfect measure of tech debt exists. But tracking things like code complexity scores, incident rates, and developer surveys gives you visibility you would not otherwise have. As Peter Drucker said: "We cannot improve what we do not measure."

## Origins

Tom Gilb, a consultant and author on software engineering, formulated this law. It complements his other work on quantifying requirements and using metrics in planning, including Planguage and evolutionary project management.

## Balance with Goodhart's Law

Gilb's Law and Goodhart's Law form a complementary pair. Goodhart warns against making metrics into targets that distort behavior. Gilb reminds us that avoiding measurement entirely leaves us blind.

The key is to use metrics for awareness, and to continuously refine what you measure.
