---
title: Postel's Law
slug: postels-law
category: Behavior
summary: Be liberal in what you accept from users and conservative in what you send back, designing interfaces that tolerate variable input while delivering predictable output.
source: https://lawsofux.com/postels-law/
---

# Postel's Law

"Be liberal in what you accept, and conservative in what you send."

## Takeaways

- Be empathetic to, flexible about, and tolerant of the various actions a user might take or input they might provide.
- Anticipate a wide range of inputs, access patterns, and capabilities while still providing a reliable and accessible interface.
- The more variability designers can plan for, the more resilient the resulting design will be.
- Accept variable input from users, translate it to meet system requirements, define clear boundaries, and give clear feedback when something is off.

## Overview

Also known as the Robustness Principle, Postel's Law treats tolerance as a design responsibility. Users type phone numbers in different formats, paste addresses with extra whitespace, abandon tasks halfway, and arrive on devices and connections the designer never tested. A system that demands exactness will frustrate them; a system that quietly normalizes their input and behaves predictably will feel forgiving and reliable. The output side matters too: while the interface accepts variability, what it returns to the user, or to other systems, should be consistent and well-formed. The combination produces interfaces that feel both flexible and dependable.

## Origins

The principle was formulated by Jon Postel, an early internet pioneer, as a design guideline for TCP and network software in the late 1970s. He wrote that programs sending messages should strictly conform to specifications, while programs receiving messages should accept non-conformant input so long as the meaning remained intelligible. The idea has since been adopted well beyond networking, becoming a foundational principle for resilient interface design.
