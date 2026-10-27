# Product & engineering roadmap

[Türkçe](ROADMAP.tr.md) · [Profile](README.md)

Updated 27 October 2026. Five usable increments were delivered sequentially. The next gates below are validation and architecture work, without delivery-date or performance promises.

| Product | Released increment | Next meaningful gate |
| :--- | :--- | :--- |
| **VoiceBridge** | [Alpha.4](https://github.com/nexora-studio-tr/voicebridge/releases/tag/v0.1.0-alpha.4): queue-inclusive per-caption timings and bilingual stage explanations. | Independent installation and two-person language, overlap, playback and consent tests. Timings exclude capture, Discord transport and browser playback. |
| **ProofGate** | [Alpha.2](https://github.com/nexora-studio-tr/proofgate/releases/tag/v0.1.0-alpha.2): read-only workspace dependency impact preflight. | Review package-bound execution/evidence architecture before implementing monorepo test execution. Current execution remains single-package npm/Vitest. |
| **ReproPack** | [0.6.0-alpha.2](https://github.com/nexora-studio-tr/repropack/releases/tag/v0.6.0-alpha.2): retained-step deletion witnesses and explicit partial certification evidence. | Durable PostgreSQL replay across registry restarts and an independent pilot. Current snapshot lifetime remains registry-bound. |
| **AccessLease** | [Alpha.2](https://github.com/nexora-studio-tr/accesslease/releases/tag/v0.1.0-alpha.2): linked renewals requiring independent approval, with unchanged original expiry. | Dedicated live Discord grant, expiry, administrator intervention and restart acceptance. This test remains deferred. |
| **Nexora FrameLab** | [Alpha.2](https://github.com/nexora-studio-tr/nexora-framelab/releases/tag/v0.1.0-alpha.2): observational comparison of imported captures with explicit quality gates. | Live CS2 replay/capture/recovery and named-hardware measurements before any tuning or FPS-gain claim. Live game testing remains deferred. |

## Current user-validation gate

VoiceBridge remains the beta focus. Two distinct people should test both language directions, overlapping speech, private playback and consent cancellation. Installation checks and per-caption stage timings help diagnosis; neither proves speech quality, end-to-end listening latency or capacity. [Join the beta](https://github.com/nexora-studio-tr/voicebridge/issues/1).

Each release includes meaningful automated checks, source/release identity, installation instructions and English/Turkish documentation. Independent human acceptance and deferred live tests are identified separately. Reproducible user feedback determines the next implementation priority.
