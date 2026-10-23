# Capabilities and honest status

[← Back to overview](../README.md)

Status reflects implementation evidence as of **22–23 October 2026**. "Live-deployed" means running on the creator's Mac; it is **not** the same as Owner-accepted (see [Milestones](milestones.md) for acceptance records). Recent work from 22–23 October is live-deployed, pending Owner acceptance.

Legend: **Live-deployed** · **Partial** (limits stated) · **Planned** (not built)

## Cybersecurity Intelligence

| Capability | Status | Today |
|---|---|---|
| Log and alert analysis | Live-deployed | Alert triage with a score and next steps; EVTX, syslog, JSON, CSV, web and cloud-audit logs |
| Network and PCAP analysis | Live-deployed | Packet-capture analysis and Wireshark labs |
| Threat detection | Partial | On logs and captures the user provides; no live monitoring of systems |
| IOC extraction | Live-deployed | Extracting and defanging indicators |
| MITRE ATT&CK mapping | Live-deployed | Local ATT&CK data, mapping, heat maps, technique teaching |
| Vulnerability prioritization | Live-deployed | CVE ranking using CISA KEV and EPSS data |
| Threat intelligence and OSINT | Live-deployed | Indicator enrichment, public lookups on request, exercises |
| Incident-response reasoning | Live-deployed | Investigation timelines, correlation, reports, IR exercises |
| Forensic reasoning | Partial | Timeline and evidence reasoning; disk and memory forensics planned |
| Sigma and detection engineering | Partial | Sigma rules on logs and practice; writing new rules planned |
| SOC analyst practice | Live-deployed | 13 hands-on exercises with hints, scoring and debriefs |
| Lab / range integration | Partial | Wireshark labs and a declared lab scope; VM-based labs planned |
| Live SOC operations, threat hunting at scale, governed security sub-agents | Planned | Later milestones |

## Human Empowerment

| Capability | Status | Today |
|---|---|---|
| Teaching and guided learning | Live-deployed | Lessons on any topic, from the user's own library first |
| Study planning, quizzes, mastery tracking | Live-deployed | Study plans, flashcards, spaced repetition, tests that prove mastery |
| Visual teaching (lightboard, 3D/HUD visuals) | Live-deployed | Visuals that build step by step as CIPHER speaks; captions on request |
| On-device image generation | Live-deployed | Pictures generated locally, no cloud |
| Research | Live-deployed | Web research with sources; reading documents the user grants |
| Productivity | Live-deployed | Timers, alarms, reminders, notes, calendar; mail and message drafts sent only after a yes |
| General computer assistance | Partial | Opening apps and sites, window arrangement, approved clicks and typing; reliable desktop and browser control not yet accepted |
| Browser and screen assistance | Partial | Navigation and read-only screen viewing; signed-in browsing and acting on the screen by sight are designed, not built |
| Accessibility | Partial | Voice-first use, read-aloud, comfort settings; validated assistive modes planned |

## Resilience

| Capability | Status | Today |
|---|---|---|
| Provider and model fallback | Live-deployed | Automatic routing across free AI services with quota handling |
| Degradation awareness | Partial | Says when a service is unavailable and continues with the next |
| System health | Partial | Health checks shown and spoken truthfully; self-repair planned |
| Operational continuity | Partial | Stable runtime copy, restart at login and after a crash, persistent memory |
| Backup and recovery reasoning, credential resilience, BIA, RTO/RPO, resilience dashboard | Planned | Later milestones |

## Not built (never claimed as done)

Moving, renaming or deleting the owner's files; owner voice lock; live SIEM/EDR or real scanning outside a declared lab; disk and memory forensics; writing new detection rules; VM-based labs; self-repair; a resilience dashboard.
