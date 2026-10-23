# Engineering milestones

[← Back to overview](../README.md)

Each milestone had a written brief, automated tests and a recorded verdict. The **Recorded result** column uses the wording of the milestone record. Automated tests passing is never treated as acceptance: a milestone closes only on the creator's live test.

## CIPHER P1 (current version)

| Milestone | Date (2026) | Scope | Recorded result |
|---|---|---|---|
| P1-00 | 27 Sep | Re-test of an off-the-shelf open-source assistant base as a foundation | **FAIL**: conversation loop, latency and reasoning did not meet requirements on the target Mac. Decision: build CIPHER P1 on its own core |
| P1-01 | 27 Sep | Local voice loop with CIPHER's own conversation layer | PASS (local target met; known gaps listed) |
| P1-02 | 27 Sep | Security core: identity, authorization, scope, approval, hash-chained evidence log | PASS; creator's live test passed (incl. a spoofed "already confirmed" being refused) |
| P1-03 | 27 Sep | Attention and silence: standby, mute, call detection, Emergency Stop, menu-bar control | PASS; creator's live test passed |
| P1-04 | 28 Sep | Identity and self-knowledge | PASS; creator's live test passed |
| P1-05 | 28 Sep | Research, documents and owner permissions; multi-brain routing; personality and voice | PASS declared by the creator after live test (10 of 11 items first time; voice item redone) |
| P1-06 | 29 Sep | Embodiment A: presence and placement on the desktop | PASS (creator's live test) |
| P1-07 | 1–5 Oct | Living embodiment and conversation core rebuild | PASS recorded after the creator's visual acceptance |
| P1-08 | 6 Oct | Study companion, memory, auto-start, approved desktop actions | Implemented and tested (585 of 586 unit tests); acceptance not recorded in the milestone report |
| P1-10A | 7 Oct | Security and access profiles (one policy engine: allow / confirm / read-only / deny) | PASS (creator, 7 Oct) |
| P1-10 | Oct | Full assistive computer control | **Open**: partial, not accepted |
| P1-11 | 8 Oct | Cybersecurity labs, exercises and analyst practice | Owner-accepted for use (experience-based acceptance, 8 Oct) |
| P1-11B | 8 Oct | Learning and visual explanation | Owner-accepted for use (experience-based acceptance, 8 Oct) |
| P1-11C | 8 Oct | Live-test fixes and context-aware visual teaching | Accepted under the same experience-based rule; issues reported from daily use |

## Since mid-October

Conversation reliability repairs, understand-first tool use, on-screen explaining (HUD key points, captions), governed desktop control steps and a paid-service credit meter have been built and deployed on the creator's Mac between 12 and 23 October 2026. Their status is **live-deployed, pending Owner acceptance** unless stated otherwise in the [Engineering Evidence portfolio](https://github.com/Cyber-Trails/CIPHER-Engineering-Evidence).

## Before CIPHER P1

CIPHER went through earlier private prototypes in August and September 2026, including Ciphlet (Raspberry Pi) and Prototype I. They are used here only for chronology; current architecture and status come from CIPHER P1.
