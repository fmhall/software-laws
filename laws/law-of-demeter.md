---
title: Law of Demeter
slug: law-of-demeter
category: Design
level: Mid-Level
summary: An object should only interact with its immediate friends, not strangers. This principle minimizes knowledge about system structure and fosters loose coupling between components.
source: https://lawsofsoftwareengineering.com/laws/law-of-demeter
---

# Law of Demeter

## Law of Demeter

"An object should only interact with its immediate friends, not strangers."

## Takeaways

- An object should only call methods of: itself, its direct components, its function parameters, or objects it creates. It should not navigate through one object to reach another ("don't talk to strangers").
- If object A only calls B (its immediate friend) and doesn't reach into B's internals (like C), then changes to C or removal of C don't affect A. Each class knows as little as possible about others, reducing the impact of changes
- It often leads to adding wrapper methods or delegations. While that might increase the number of methods, it results in cleaner interactions.

## Overview

The Law of Demeter, also known as "don't talk to strangers" or the "principle of least knowledge," was formulated to minimize the knowledge that any given object has about the overall system structure.

In practice, if object A has a reference to object B, and B has a reference to C, A should not call methods on C through B (like `a.b.getC().doSomething()`). A can talk to B, and B can talk to C, but A shouldn't directly get involved with C.

This fosters loose coupling. If you break LoD, your code assumes the structure extends beyond its immediate neighbors. For example, if `OrderProcessor` does `order.getCustomer().getAddress().getZipCode()`, it knows that an Order has a Customer with an Address. If Customer is changed to have multiple addresses, OrderProcessor breaks. If instead Order had a method `getShippingZip()` that internally navigates its customer/address, OrderProcessor could call that and be oblivious to structural changes.

LoD aligns with information hiding: each object hides its internals and only exposes necessary interfaces.

## Examples

Consider a `Presenter` object with a reference to a UI View containing a `TextField`. Without LoD, the presenter might do `view.getTextField().setText("Hello")`. LoD encourages View to provide `setUserMessage(String)`, internally calling `textField.setText`. The Presenter doesn't need to know there's a TextField specifically. If later the View uses a Label instead, the Presenter code doesn't change.

You can identify violations by counting dots: `a.getB().getC().doSomething()` has two dots, one too many. A single dot `a.doSomething()` or at most `a.getB().doSomething()` is preferable.

By adhering to LoD, each component remains more self-contained, and systems become a network of "friends" rather than a tangle of strangers reaching through each other.

## Origins

The Law of Demeter was first described around 1987 by Ian Holland and colleagues at Northeastern University as part of the Demeter Project on adaptive and aspect-oriented software development. It's named after the project, which itself was named after the Greek goddess of agriculture, signifying a "growing" approach to software.

The researchers, including Karl Lieberherr, sought ways to make software more maintainable and developed this style rule. They summarized it with the motto "Only talk to your friends."
