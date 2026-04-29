---
title: Hyrum's Law
slug: hyrums-law
category: Architecture
level: Senior
summary: With sufficient API users, all observable system behaviors become dependencies, even unintended ones. This blurs the line between documented interface and implementation details.
source: https://lawsofsoftwareengineering.com/laws/hyrums-law
---

# Hyrum's Law

"With a sufficient number of API users, all observable behaviors of your system will be depended on by somebody."

## Takeaways

- As the user count grows, everything your system does becomes a dependency point. Even unintended side effects or bugs can become 'features' that someone's workflow depends on.
- Hyrum's Law warns maintainers that any change can break something for someone. Consumers may have integrated your API in ways you didn't expect, including relying on timing, error messages, formatting, etc.
- The actual contract of your software isn't just the official API/spec; it's the exact behavior as observed in the wild. The contract can even be something informal, such as the UI that your users are used to.

## Overview

Hyrum's Law describes a phenomenon where the boundary between a software's documented interface and its implementation details gets blurred in practice. No matter what you promise in an API contract, if people use your system enough, they will depend on behaviors you never officially supported.

Over time, the implementation becomes the interface. Every observable trait, performance characteristic, or error code might be assumed by someone. This drastically limits freedom to change the system, as even internal changes can break users who wrote code around the old behavior.

## Examples

**Microsoft Windows** had undocumented behaviors and bugs that many third-party applications relied on. When Microsoft fixed or changed those behaviors in new versions, those applications broke. Microsoft often had to revert or maintain quirky behavior to ensure compatibility.

A **library** might state in the docs that a function returns an unordered list, but it currently returns a sorted list. Some users start depending on it being sorted. If the library later changes to truly unordered, those users' code will break. The law is especially relevant in API versioning: even minor changes can be breaking changes from someone's perspective.

## Origins

The law is named after **Hyrum Wright**, a software engineer who articulated this observation while at Google around 2011-2012. Hyrum noticed that even changes to core Google libraries that should have been invisible would often break some project somewhere, because that project relied on an undocumented behavior.

His colleague, Titus Winters, coined the term "Hyrum's Law" in recognition of it (in Software Engineering at Google).
