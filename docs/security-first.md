# Security first

[← Back to overview](../README.md)

## The principle

CIPHER is an assistant that can act on a real computer: open apps, send messages after approval, read documents, run analyses. That makes it a security system first and a helpful assistant second. Before CIPHER's capabilities were expanded, its security foundation was built and tested (milestone P1-02, 27 September 2026).

Four ideas run through the design:

1. **The model suggests; code decides.** Every action CIPHER's AI model proposes becomes a tool call that passes a policy and authorization check before it can run. Model output is never treated as permission.
2. **Fail closed.** If a check cannot be completed, the action does not happen.
3. **Human authority for consequential actions.** Destructive or external actions (for example, submitting a form or sending a message) are read back and wait for the owner's live confirmation.
4. **Executed is not verified.** An action is reported as done only when its outcome has been checked, and every decision is written to a tamper-evident evidence log.

Voice engagement is not authentication: hearing the owner's voice does not grant authority by itself.

## The fourteen foundational controls

CIPHER has **14 foundational controls (C-01 to C-14)**. Some internal documents group them into five bundles; the bundles are groupings of the same 14 controls, not additional controls. (Some earlier documents said 13; the authoritative control register lists 14.)

Status below is from a runtime coverage review dated **22 October 2026**, which re-checked three days of evidence records: **169 actions, 169 of 169 with a recorded policy and authorization decision**, and an evidence chain of **50,393 records, intact**.

| # | Control | Purpose | Status (22 Oct 2026) |
|---|---|---|---|
| C-01 | Identity | Only CIPHER's own identity acts | Verified in live use |
| C-02 | Authentication / Owner Gate | Owner authority is required and fails closed | Verified in live use (stronger step-up authentication planned) |
| C-03 | Capability / authorization | Every action gets a policy and authorization decision | Verified in live use |
| C-04 | Operational scope | Every action carries a scope (read-only, local write, destructive, external network) | Verified in live use |
| C-05 | Autonomy | Autonomous action needs explicit delegation | Implemented; **not yet exercised in live use** |
| C-06 | Policy / risk | Forbidden actions are blocked before anything else runs | Implemented and unit-tested; not triggered in live use |
| C-07 | Human authorization / safe preview | Consequential actions are read back and need live confirmation | Verified in live use |
| C-08 | Delegation | Delegated agents get read-only authority | Implemented; **not fully live-verified** (no delegation used yet) |
| C-09 | Blast-radius control | Limits how much one request can do | **Needs re-validation** for multi-step tasks |
| C-10 | Secure execution | Actions run so they can be stopped; Emergency Stop | Verified in live use |
| C-11 | Outcome verification | "Executed" is not "verified" | **Partial**: one case reported success after an app error; fix planned |
| C-12 | Audit / evidence | Hash-chained, redacted, verifiable evidence log | Verified in live use |
| C-13 | Containment / recovery | Emergency Stop, hard mute (microphone closed), standby | **Partial**: stop and hard mute work; full compromise recovery not yet built |
| C-14 | Untrusted input / prompt injection | Web, email and screen content is treated as data, not instructions | **Needs re-validation** since the AI model began choosing tools (every call is still policy-gated) |

**Summary:** 7 controls verified in live use, 1 verified in code and tests, 2 implemented but not yet exercised live, 4 partial or awaiting re-validation. None of the 14 is described as complete for a public release until those four are closed and a dedicated security validation lab has passed.

## Privacy by design

- **Mute means the microphone is closed**, not merely that CIPHER stops talking.
- A visible privacy switch keeps CIPHER local-only (no cloud, no memory writes).
- Speech heard in standby or after mute is discarded at the boundary; a defect where this failed was treated as a security issue ([case study CE-22](https://github.com/Cyber-Trails/CIPHER-Engineering-Evidence/blob/main/case-studies/CE-22-private-audio.md)).
- Paid AI services are used only when the owner asks, under a spending limit.

## What is deliberately not published

Rule lists, enforcement code, approval mechanics, credential handling and unpublished weaknesses stay private. This page describes *what* the controls do and *how well they are verified*, not *how* to get around them.
