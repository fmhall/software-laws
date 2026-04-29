---
title: Cunningham's Law
slug: cunninghams-law
category: Decisions
level: Junior
summary: The best way to get correct answers online is to post a wrong answer rather than ask a question, as people are motivated to correct errors. This principle applies to software engineering by encouraging concrete proposals over abstract inquiries.
source: https://lawsofsoftwareengineering.com/laws/cunninghams-law
---

# Cunningham's Law

## Cunningham's Law

"The best way to get the correct answer on the Internet is not to ask a question, it's to post the wrong answer."

## Takeaways

- People online love correcting errors. If you're stuck on a problem, sometimes proposing a solution (even if it might be wrong) can get you to the right solution faster.
- Asking a question might evoke only silence, but confidently stating something (even if incorrect) often provokes a reaction.
- Instead of endlessly asking "How should we do X?", propose a draft or prototype. Even if it's not entirely correct, having a concrete starting point often gets more feedback ("No, not like that, do it this way").

## Overview

Cunningham's Law arose in the context of online communities, particularly wikis and forums. The underlying observation is that assertions draw more engagement than questions. On Wikipedia, if someone posts incorrect information, other editors will rush in to fix it.

In software engineering, you see this on Stack Overflow and mailing lists. A user asks a question and gets few responses, but if someone posts a slightly wrong answer, others quickly chime in to correct it. By putting something out there, you transform a passive question into an active discussion.

## Examples

A developer stuck on configuring an open-source library posts a question and gets no replies. Using Cunningham's Law, they post: "For anyone else struggling, the solution is to set ConfigMode to False." If wrong, someone (possibly the library maintainer) will quickly reply: "Actually, no, you should leave ConfigMode true, it's another setting you need to change."

A new developer uncertain about implementing a feature submits a pull request with their best attempt rather than asking in the abstract. Senior engineers review it and point out improvements. By presenting a "proposed answer," the developer gets the team's knowledge and ends up with the right approach.

## Origins

Cunningham's Law is named after Ward Cunningham, the American programmer best known for creating the first wiki software. The actual phrasing of the law is often attributed to a colleague of Cunningham, Steven McGeady, who formulated the adage and named it after Cunningham.

According to McGeady, Ward Cunningham gave him advice in the 1980s regarding early internet forums (Usenet), and McGeady later described it in a comment on a New York Times blog in 2010.

The irony is that Ward Cunningham's invention, the wiki, is a platform built precisely on the idea that people will collaboratively correct and improve content.

The French have a proverb, "Prêcher le faux pour savoir le vrai" (preach the false to know the true), which captures a similar concept.
