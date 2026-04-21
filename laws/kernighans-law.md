---
title: Kernighan's Law
slug: kernighans-law
category: Quality
level: Junior
summary: Debugging is twice as hard as writing code because it requires understanding both what code does and why it fails. Writing overly complex code creates problems for future maintenance and troubleshooting.
source: https://lawsofsoftwareengineering.com/laws/kernighans-law
---

# Kernighan's Law

## Kernighan's Law

Debugging is twice as hard as writing the code in the first place.

## Takeaways

- Bug detection and removal is more complex than programming because debugging requires understanding both the code and why it doesn't work.
- If you write code at the limit of your intelligence, you won't be able to understand or troubleshoot it later.
- Simple code with good structure and documentation is easier to debug, saving time in the long run.
- Even if your code runs successfully when you write it, it's fragile if it's too complex.

## Overview

Kernighan's Law says that debugging requires understanding what the code _actually_ does, which can be twice as hard as writing it. When coding, you operate with a specific mental model and full context. When debugging, you might be dealing with someone else's code or your own code after that context has faded.

Writing "clever" or complex code is essentially setting a trap for your future self. A maintainable version is usually superior to an optimized version that is difficult to understand. As Kernighan implies, if you make your code too tricky, you've essentially outsmarted yourself.

## Examples

Imagine a developer writing a function in a compressed style, chaining multiple operations in one line:

```
public string GetUserDisplay(User u) =>
     u?.IsActive == true ? (u.Name ?? "").Trim() is var n && n.Length > 0
     ? n + (u.Role > 0 ? $" ({(Role)u.Role})" : "") : "Unknown" : "Inactive";
```

The proper, readable version:

```
public string GetUserDisplay(User user)
{
    if (user is null || !user.IsActive)
        return "Inactive";

    var name = user.Name?.Trim();

    if (string.IsNullOrEmpty(name))
        return "Unknown";

    if (user.Role > 0)
        return $"{name} ({(Role)user.Role})";

    return name;
}
```

The clever version might have taken 30 minutes to write, but debugging took 3 hours. Had the code been written clearly, it would've taken 45 minutes to write, but only 30 minutes to debug later.

## Origins

Brian Kernighan first expressed this idea in _The Elements of Programming Style_ (1974, second edition 1978) with P.J. Plauger. Kernighan, famous for co-authoring "The C Programming Language" and "The Elements of Programming Style," wrote about simplicity in the days of resource-constrained computing.
