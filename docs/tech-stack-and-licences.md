# Tech stack and third-party licences

[← Back to overview](../README.md)

CIPHER is a **private, personal, non-commercial** project. Its code is not distributed. The main third-party components it uses are listed here for transparency and credit; this is not an exhaustive dependency list.

| Area | Component | Licence |
|---|---|---|
| Languages / platform | Python; Swift and AppKit on macOS | n/a |
| Conversation pipeline | Pipecat | BSD-2-Clause |
| Speech recognition (local) | faster-whisper | MIT |
| Speech synthesis (local) | Kokoro (kokoro-onnx runtime) | MIT (runtime); model licence per its model card |
| Speech synthesis, phonemes | phonemizer, espeak-ng | **GPL-3.0-or-later** |
| Speech synthesis, fallback voice | piper-tts | **GPL-3.0-or-later** |
| Model runtime | ONNX Runtime | MIT |
| Local AI models | Ollama | MIT |
| Paid AI service (on owner request only) | Anthropic API (Python SDK) | MIT (SDK) |
| Memory | Mem0, Qdrant client | Apache-2.0 |
| Spaced repetition | fsrs | MIT |
| Web research | trafilatura, ddgs, httpx | Apache-2.0, MIT, BSD-3-Clause |
| macOS integration | PyObjC | MIT |
| On-device image generation | mflux; FLUX.1 [schnell] weights | MIT; Apache-2.0 |
| HUD and visuals | three.js, D3, ECharts, Mermaid, KaTeX, highlight.js, Rough.js | Permissive (MIT / Apache-2.0 / BSD-style, licence files bundled) |

## GPL components

`piper-tts`, `phonemizer` and `espeak-ng` are GPL-licensed and sit in CIPHER's speech path. Private, personal use is permitted. CIPHER is not distributed; before any distribution or commercial use they would be replaced with permissively licensed alternatives or the GPL would be fully complied with.

## Creative assets

Original design by the Owner (hand sketches), AI-assisted digitization, then Owner-directed iterative refinement to the final approved form. The embodiment artwork is all rights reserved and is not licensed for reuse; see [Origin & authorship](origin-and-authorship.md).

Licences above were read from installed package metadata on 23 October 2026.
