# Ciphlet Prototype 1 | Raspberry Pi AI Learning Companion

**Prototype 1 — operational build, currently not powered on • Public engineering case study**

Ciphlet Prototype 1 is the first working Raspberry Pi 5 implementation of **CIPHLET** (Cybersecurity Intelligent Personal Helper for Learning, Exploration & Training), a voice-first AI cybersecurity learning companion. Its purpose was to demonstrate a physical assistant with local/cloud intelligence, conversation and voice integration. The underlying prototype remains intact; the external JUNEBOX display enclosure was returned and is not part of the claimed final hardware configuration.

This public showcase is a **portfolio of documented engineering achievements**, not an open-source software distribution. The private source repository remains private.

## Prototype 1 — documented stages

| Stage | Work performed | Evidence / distinction |
|---|---|---|
| 1 — Hardware assembly | Raspberry Pi 5, cooling, storage and peripherals | Original hardware photographs |
| 2 — Physical integration | Fit, cable routing, cooling and candidate display configuration | Assembly photographs; the candidate enclosure was not adopted |
| 3 — Linux/software bring-up | Python installation, project transfer and Ciphlet CLI | CLI and terminal evidence |
| 4 — Real conversation | Ciphlet handled interactive text conversations | Runtime terminal screenshots and live test reports |
| 5 — Hybrid/local brain | Model/provider routing; Pi-verified Ollama local inference | Accepted Gemma 3 1B, persistent local Ollama, streaming and bounded context |
| 6 — Voice pipeline | Microphone, VOSK STT, Piper TTS, wake-word experiments, hands-free loop | Pi testing demonstrated wake→capture→transcribe→brain→speech and repeated turns; reliability limits recorded |
| 7 — Troubleshooting & hardening | USB sample-rate mismatch, self-hearing echo, turn continuity, wake calibration | Failures diagnosed and fixes validated with real Pi test evidence |

### What was actually proven

- **Physical engineering:** the owner assembled and integrated the Raspberry Pi 5 hardware and peripherals.
- **Local intelligence:** a persistent Ollama server with `gemma3:1b-it-q4_K_M` produced Pi-verified local-only responses with streaming and bounded context.
- **Voice function:** real Pi tests established microphone capture, VOSK transcription, Piper-to-speaker output, push-to-talk and a multi-turn hands-free processing loop. Earlier live tests used an available diagnostic wake phrase; the intended custom “Hey Ciphlet” wake phrase still required tuning for reliable everyday use.
- **Engineering judgment:** audio hardware, echo, model selection, wake detection and memory-context defects were investigated, tested and documented instead of declared solved based only on code or mock tests.

**Do not confuse functional voice tests with a fully polished hands-free product:** noisy environments, echo sensitivity, interruption quality and general wake-word reliability remained development concerns.

## What I learned

1. **Verify on physical hardware.** A software test passing on the development Mac does not establish Pi compatibility.
2. **Diagnose from runtime measurements.** The microphone’s sample-rate limitations, acoustic echo and conversation timing each required different evidence.
3. **Separate memory storage from model behavior.** Correctly persisting and passing conversation history does not ensure an LLM uses it accurately.
4. **Design for constrained computing.** CPU, RAM, thermal headroom and audio latency drive realistic deployment decisions.
5. **Protect the boundary between public evidence and private code.** Screenshots, API credentials, configuration and internal implementation need screening before publication.

## Portfolio materials

A 12-slide **Ciphlet Prototype 1 portfolio presentation** and a Word-format development journey have been prepared, with original user-supplied photos and technical takeaways. Files are supplied separately until approved binary assets can be added here. The photo gallery is pending binary upload.

## Prototype boundary

**Prototype 1** is the intact working prototype documented here. **Prototype 2** is a distinct successor build planned around Pironman hardware; its future milestones will not be represented as Prototype 1 achievements. Ciphlet remains architecturally independent of CIPHER.

[Back to CIPHER Showcase](../README.md)
