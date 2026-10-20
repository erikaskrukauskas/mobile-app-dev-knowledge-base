---
title: Mobile application security
tags: [practices, security, permissions, mobile]
status: verified
updated: 2026-10-19
---

# Mobile application security

Treat three mobile concerns as part of the design: platform permissions, data on the device, and secrets kept out of git. Security that any client could use — input handling on a server, a public authentication boundary, token audience — lives in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base). Link that page for the general rule, and keep the device-specific rule here.

## Platform permissions

Ask for a permission at the moment the person can see why it is needed. Name the capability the screen requires, the behavior when the person allows it, and the behavior when they deny it or have already denied it.

A denied permission is a specified outcome, not an exception to hide. The screen still has to offer a path the person can understand. See [Specify the screen and done](02-specify-screen-and-done.md).

The platform decides how the prompt looks and how a previous denial is remembered. Confirm the current page for that platform in [Official-Documentation/README.md](../Official-Documentation/README.md) before relying on a prompt, a settings deep link, or a permission state. This page does not choose iOS or Android as the practice.

## Data on the device

Say what the app stores on the device, how long it stays, and who else on the device can read it. Local state that includes personal data, credentials, or offline copies of private records needs an explicit boundary: what is stored, what is shown on screen, and what is removed when the person signs out or the data is no longer needed.

Offline behavior and local state are part of this boundary. A queue of commands waiting for the network can contain the same sensitive data as the screen that created it. Name that store in the screen contract.

Prefer the platform's protected storage for secrets and tokens that must remain on the device. Confirm the current protected-storage page before naming an API. Do not invent a home-grown store for secrets when the platform already provides one you have confirmed.

## Secrets kept out of git

Keys, tokens, passwords, and store-account credentials do not belong in this repo or in a mobile project's source. `.gitignore` in this library ignores `.env` and `.env.*` as a backstop. A project still has to keep its own secrets out of its repository.

A sample, a screenshot, and a lesson must use placeholders. If a check requires a real secret, say where the project stores it. Do not paste the value.

## Check

The check for a permission or for data on the device runs on a mobile client: allow, deny, and the signed-out or offline case that the specification named. Record a lesson here when that device behavior would help another mobile project.
