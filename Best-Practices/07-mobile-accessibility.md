---
title: Mobile accessibility
tags: [practices, accessibility, screen, mobile]
status: verified
updated: 2026-10-19
---

# Mobile accessibility

A person must be able to perceive, operate, and understand the mobile client on a phone. Name that commitment in the screen contract, and check it on a mobile client. A desktop-only check does not show that the phone path works.

## Perceive

The person can tell what the screen contains without relying on a single sense. Text and controls have names a screen reader can speak. Information that is shown by color is also shown by text or shape. Contrast and text size remain usable on a phone screen, including when the person enlarges text.

## Operate

The person can complete the journey with the input methods the platform provides, including a screen reader and a switch or keyboard when the platform offers them. Touch targets are large enough to hit. Navigation still has a way back. A control that cannot be reached by the assistive technology the platform provides is unfinished.

Time limits, gestures that have no alternative, and actions that fire on touch-down are called out in the screen contract when the screen uses them.

## Understand

Labels say what the control does. Errors say what failed and what the person can do next, in the same place as the other mobile error handling for that screen. Focus moves to the error or the error is announced. The screen does not rely on placeholder text alone to name a field.

## Specify and check

Include the accessibility behavior in [Specify the screen and done](02-specify-screen-and-done.md): what a screen reader announces, which controls are reachable, and the path someone exercises on a phone with the platform's assistive technology turned on.

Confirm the current accessibility guidance before relying on a platform feature or a success criterion. Entry points, including WCAG and the platform guides, are in [Official-Documentation/README.md](../Official-Documentation/README.md). This page does not pick a platform or a framework as the practice.

## Relationship to other libraries

Interface research and visual design that are not specific to a phone stay with the product or with the interface library that project uses. A general application accessibility rule that does not depend on a mobile client is linked from the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base) when that page is the canonical rule. The phone-specific commitment stays here.
