---
title: Principle of Least Astonishment
slug: principle-of-least-astonishment
category: Design
level: Mid-Level
summary: Software and interfaces should behave in ways that least surprise users and other developers, aligning with their expectations and standard conventions.
source: https://lawsofsoftwareengineering.com/laws/principle-of-least-astonishment
---

# Principle of Least Astonishment

## Principle of Least Astonishment

Software and interfaces should behave in a way that least surprises users and other developers.

### Takeaways

- Design decisions should align with user expectations. When someone uses a component (a UI element, API, etc.), its behavior should not be surprising or counterintuitive.
- Following platform norms or standard conventions yields the least astonishment.
- In practice, it improves usability and developer experience. Users can predict how to interact with the software, and developers can predict how to use an API by analogy with similar ones. Surprises often lead to mistakes.

### Overview

The Principle of Least Astonishment (POLA) is a general design principle in user interface design, software API design, coding, and documentation. The idea is simple: don't surprise the user.

The system should behave in a way that matches the user's mental model of how it ought to work. Violating this principle doesn't necessarily break functionality, but it breaks trust and ease of use.

In coding, this principle states that your code should behave as the developer expects when name, type, and context are taken into account. We should choose defaults and behaviors that match standard conventions and avoid "surprise" side effects.

### Examples

In software APIs, POLA means designing functions and behaviors that meet standard expectations. If you have a method `deleteFile()`, one would expect it to remove the file. It should not secretly archive it or throw an error if the file doesn't exist.

If your method works similarly to a well-known one in another library, keep naming and behavior aligned. A `toString()` method should return human-readable text, not a binary blob.

POLA also covers error handling and defaults. Sensible defaults cause the least surprise. For developers, code surprises are equally problematic. If a function `parseDate(str)` internally modifies a global date format setting, that's surprising.

Following standard naming conventions matters: a variable named `isReady` should be boolean, a function named `compute` should return something rather than modify global state.

A delighted user or developer uses something and it "just works" as expected.

### Origins

The concept of least astonishment has roots in early human-computer interaction. An early mention appears in PL/I programming language documentation around 1967, complaining that certain behaviors violated the principle.

The principle was explicitly stated in a 1972 publication on programming language design, recommending that language constructs behave as their syntax suggests and follow widely accepted conventions.

Since then, it has been emphasized across various domains. In the Unix community, Eric Raymond's Art of Unix Programming references it as the "Rule of Least Surprise."
