<div align="center">

**@CIPHER**

# CIPHER
### Cybersecurity Intelligence Platform for Human Empowerment and Resilience

**Security-first AI engineering | Human authority | Evidence over claims**

*An independently developed, voice-first AI assistant for macOS, built so that every action it takes is checked, recorded and, where it matters, approved by its owner.*

[Overview](#what-cipher-is) · [Security first](docs/security-first.md) · [Architecture](docs/architecture.md) · [Capabilities](docs/capabilities.md) · [Milestones](docs/milestones.md) · [Lessons](docs/lessons-learned.md) · [Roadmap](docs/roadmap.md) · [Tech stack](docs/tech-stack-and-licences.md) · [Origin & authorship](docs/origin-and-authorship.md)

</div>

---

## What CIPHER is

CIPHER is a persistent, security-first AI assistant that runs on its owner's Mac. It talks and listens, teaches, researches with sources, helps with cybersecurity analysis and practice, and carries out computer tasks, always inside a governance layer that decides what it may do.

Its design motto: **one CIPHER platform, three capability domains, one security and governance control plane.**

| Capability domain | What it covers today |
|---|---|
| **Cybersecurity Intelligence** | Log and alert analysis, packet-capture labs, IOC extraction, MITRE ATT&CK mapping, vulnerability prioritization, threat-intelligence and incident-response exercises |
| **Human Empowerment** | Tutoring and study planning, quizzes and mastery tracking, visual teaching on a holographic HUD, research with citations, productivity |
| **Resilience** | Provider fallback when an AI service is down, honest degradation reporting, health checks, restart and recovery basics |

Detail and honest status for each area: [Capabilities](docs/capabilities.md).

## Why security comes first

CIPHER's security foundation was built **before** its capabilities were expanded. The AI model may *suggest* an action; code decides whether it runs. Fourteen foundational controls cover identity, authorization, scope, risk, human approval, execution, outcome checks, a tamper-evident evidence log, containment and untrusted input. Destructive or external actions wait for the owner's spoken confirmation, and an Emergency Stop and hard mute are always available.

Their current status is published as it stands, including the gaps: [Security first](docs/security-first.md).

## How it was built

- **Independent development.** CIPHER P1 is independently engineered according to its owner-defined requirements, with a security-first core and owner-verified milestones.
- **Owner-directed, AI-assisted engineering.** The creator sets requirements, makes the security and privacy decisions, runs live acceptance tests and approves or rejects every outcome. Claude-based AI coding agents write the implementation and automated tests and perform log and code analysis. The [Engineering Evidence portfolio](https://github.com/Cyber-Trails/CIPHER-Engineering-Evidence) documents that split case by case.
- **Milestone discipline.** Each milestone has a written brief, automated tests, a recorded verdict and a known-good rollback point. Passing tests is not the same as acceptance: only the owner's live test closes a milestone. See [Milestones](docs/milestones.md).

## Status vocabulary used on these pages

| Label | Meaning |
|---|---|
| **Owner-accepted** | The creator tested it live and recorded acceptance |
| **Live-deployed, pending Owner acceptance** | Running on the creator's Mac; acceptance not yet recorded |
| **Implemented / tested** | Built and covered by automated tests; not yet proven in live use |
| **Partial** | Part of the capability works; the limits are stated |
| **Planned** | A development goal, not a completed capability |

## Showcase media

The creator has finalized a **Security-First introduction video**, a **CIPHER origin article** and an approved **SOMA still image**. They will be published here unmodified once the exact files and publication URL are confirmed and checked for unintended disclosures.

*Media publication pending asset confirmation. No substitute artwork or altered versions will be used.*

How the embodiment was designed, from the Owner's hand sketches to the final form: [Origin & authorship](docs/origin-and-authorship.md).

## Ciphlet Prototype 1 — Raspberry Pi AI Learning Companion

Ciphlet Prototype 1 is an intact, functioning Raspberry Pi 5 AI learning-companion prototype. The owner assembled the hardware, configured a Python-based runtime, validated local AI through Ollama, and tested speech recognition, spoken responses and multi-turn conversation on the real Pi. Production-level wake reliability and interruption behavior remained engineering work rather than blanket claims of completion.

[View Prototype 1 development stages, verified achievements and takeaways](docs/ciphlet-build-journey.md). A separate Pironman-based **Prototype 2** is planned. Ciphlet’s proprietary source repository remains private.


## What this repository is (and is not)

This is a **public portfolio**, not a software distribution. CIPHER's source code, security-control implementations, prompts, voice design, embodiment production files, configuration and personal data are private and are not published here.

## Creator

**Cyber-Trails** · cybersecurity and AI engineering portfolio
[GitHub profile](https://github.com/Cyber-Trails) · [Engineering Evidence](https://github.com/Cyber-Trails/CIPHER-Engineering-Evidence) · [Publication status](PUBLICATION_STATUS.md)

---

*@CIPHER · CIPHER™ · © 2026 MILDRED OWENS. All rights reserved. The embodiment artwork is all rights reserved and is not covered by any software licence. The text and media in this repository are shared for viewing only; no licence to reuse CIPHER's name, design or materials is granted. Third-party components are credited in [Tech stack and licences](docs/tech-stack-and-licences.md).*
