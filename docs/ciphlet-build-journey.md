# Ciphlet | Building a Raspberry Pi AI Companion

**A CIPHER companion project · Hardware assembly, local intelligence and cybersecurity learning**

Ciphlet is an independently developed Raspberry Pi 5 companion project within the CIPHER ecosystem. It explores a small-footprint AI learning interface, including on-device models, persistent conversations, audio interaction, and security-conscious system design.

This public engineering narrative documents **selected real-world milestones and lessons**. It is not a release of Ciphlet's private source code.

## Development journey

| Stage | Evidence and work | What was established |
| --- | --- | --- |
| 1. Hardware preparation | Raspberry Pi 5 (8 GB), peripherals, board and cooling-component assembly | Hands-on hardware integration |
| 2. Enclosure and storage | Pi fitted in a touchscreen enclosure; cooling, power and NVMe components evaluated | Physical integration and resource constraints |
| 3. Software bring-up | Linux terminal, SSH transfers, Python environment, Ciphlet CLI with `chat` and `voice` commands | Installation and command entry points |
| 4. First Pi text response | Ciphlet answered a user greeting through the Pi terminal | Real interactive *text* conversation was demonstrated |
| 5. Provider identity verification | An inaccurate model self-description was investigated and checked against serving-provider records | Runtime evidence matters more than a model's self-report |
| 6. Local AI | A lightweight Gemma 3 1B model through Ollama is recorded as Pi-verified in the repository's accepted local-brain baseline | Local-only operation, bounded history and streaming; verify latest baseline before comparisons |
| 7. Voice experiments | Speech output and device troubleshooting were documented; full hands-free reliability remained a separate validation task | Spoken output is not the same as fully verified natural conversation |

## Hands-on work and engineering lessons

The project required assembling real hardware, setting up and operating the Pi, transferring and launching software, investigating errors, evaluating resource limits and accepting or rejecting test outcomes. Software implementation and testing were supported by AI coding tools, while the project owner directed requirements, hardware work and live verification.

**Lessons learned:**
- Test on the **actual device**; code inspection is not equivalent to Pi hardware validation.
- Preserve failures as evidence: configuration, audio and database errors teach as much as successes.
- Verify provider/model identity through runtime observations, not generative self-description.
- Design for RAM, CPU, heat, storage and audio limitations.
- Keep private implementation, credentials, logs and sensitive design material out of public showcases.

## Selected photo evidence

Original photographs document the Pi board, cooler handling, open enclosure assembly, NVMe-related hardware integration, and development workbench. Sanitized images are being prepared for the gallery; **do not upload screenshots showing .env files, API keys or local identifiers**.

## Honest status

**Active prototype.** Some foundation and local-model tests are hardware verified. Other audio, interaction and educational features remain partial, under test or planned. The presence of a CLI option or an implementation file alone does not mean end-to-end feature verification.

## Relationship to CIPHER

Ciphlet is a companion project exploring small-device AI and cyber education alongside the CIPHER platform. The private development repository remains private. No CIPHER security-core internals, voice recipes or confidential implementation files are distributed here.

[Return to CIPHER Showcase](../README.md)
