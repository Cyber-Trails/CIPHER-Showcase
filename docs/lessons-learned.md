# Lessons learned

[← Back to overview](../README.md)

Short engineering lessons from building CIPHER. Detailed case studies, with a clear split between the creator's own decisions and the work done by AI coding agents, are in the [Engineering Evidence portfolio](https://github.com/Cyber-Trails/CIPHER-Engineering-Evidence).

| Lesson | What happened | Case study |
|---|---|---|
| **Convincing is not trustworthy** | An AI assistant can sound capable while doing the wrong thing. CIPHER's controls exist so that what it *does* is bounded, checked and recorded, whatever it *says*. | [Security first](security-first.md) |
| **Executed is not verified** | An action once reported success after the app had returned errors. Outcome verification became an explicit control (C-11), still marked partial. | [Security first](security-first.md) |
| **Passing tests is not acceptance** | A dashboard passed its tests but failed live review; investigation then found invented metrics. Truthful output became a requirement. | [CE-18](https://github.com/Cyber-Trails/CIPHER-Engineering-Evidence/blob/main/case-studies/CE-18-fabricated-dashboard.md) |
| **Understand intent before acting** | A keyword rule opened a dashboard when the creator only wanted to talk about it. CIPHER moved to understand-first tool use, keeping keywords decisive only for safety controls. | [CE-23](https://github.com/Cyber-Trails/CIPHER-Engineering-Evidence/blob/main/case-studies/CE-23-intent-and-permissions.md) |
| **Privacy failures are security failures** | Speech heard during standby or after mute was treated as a security defect and fixed to fail closed. | [CE-22](https://github.com/Cyber-Trails/CIPHER-Engineering-Evidence/blob/main/case-studies/CE-22-private-audio.md) |
| **Least privilege over convenience** | A broad OS permission for a convenience hotkey was declined and the feature deferred. | [CE-01](https://github.com/Cyber-Trails/CIPHER-Engineering-Evidence/blob/main/case-studies/CE-01-least-privilege.md) |
| **Question the test, not only the result** | A voice-enrollment check rejected the owner in a silent room; the test itself was wrong. | [CE-10](https://github.com/Cyber-Trails/CIPHER-Engineering-Evidence/blob/main/case-studies/CE-10-invalid-biometric-check.md) |
| **Control the test environment** | A desktop-automation test ran while the creator was using the same Mac; it was rerun under controlled conditions and still fell short of its target, so it was not accepted. | [CE-30](https://github.com/Cyber-Trails/CIPHER-Engineering-Evidence/blob/main/case-studies/CE-30-test-environment.md) |
| **Know your supply chain** | Dependencies can be abandoned or relicensed. A dependency inventory and fallback plan were created, and a licence review later corrected the project's own records. | [CE-29](https://github.com/Cyber-Trails/CIPHER-Engineering-Evidence/blob/main/case-studies/CE-29-dependency-continuity.md) |
| **A failed foundation is a result** | An off-the-shelf assistant base failed its re-test (P1-00). Recording that honestly led to building CIPHER P1 on its own core. | [Milestones](milestones.md) |
