# Product & engineering roadmap

[Türkçe](ROADMAP.tr.md) · [Profile](README.md)

Updated 29 October 2026. Five products have tagged alpha releases. VoiceBridge is the current quality and beta focus; ProofGate is the next major development. One major feature packet runs at a time.

| Product             | Released increment                                                                                                                                                                   | Next meaningful gate                                                                                                                                   |
| :------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------- |
| **VoiceBridge**     | [Alpha.7](https://github.com/nexora-studio-tr/voicebridge/releases/tag/v0.1.0-alpha.7): operator performance view, private numeric reports, safe room recovery and Windows launcher. | Repeatable TR/EN quality baseline, then evidence-led improvements. Independent installations and owner-run live acceptance are recorded separately.    |
| **ProofGate**       | [Alpha.2](https://github.com/nexora-studio-tr/proofgate/releases/tag/v0.1.0-alpha.2): read-only workspace dependency impact preflight.                                               | Review package-bound execution/evidence architecture before implementing monorepo test execution. Current execution remains single-package npm/Vitest. |
| **ReproPack**       | [0.6.0-alpha.2](https://github.com/nexora-studio-tr/repropack/releases/tag/v0.6.0-alpha.2): retained-step deletion witnesses and explicit partial certification evidence.            | Durable PostgreSQL replay across registry restarts and an independent pilot. Current snapshot lifetime remains registry-bound.                         |
| **AccessLease**     | [Alpha.2](https://github.com/nexora-studio-tr/accesslease/releases/tag/v0.1.0-alpha.2): linked renewals requiring independent approval, with unchanged original expiry.              | Dedicated live Discord grant, expiry, administrator intervention and restart acceptance. This test remains deferred.                                   |
| **Nexora FrameLab** | [Alpha.2](https://github.com/nexora-studio-tr/nexora-framelab/releases/tag/v0.1.0-alpha.2): observational comparison of imported captures with explicit quality gates.               | Live CS2 replay/capture/recovery and named-hardware measurements before any tuning or FPS-gain claim. Live game testing remains deferred.              |

## Current focus and sequence

1. **VoiceBridge: establish the quality baseline.** Compare 30 Turkish and 30 English reference phrases with documented source/model identities. Label synthetic samples; report recognition errors and critical translation meaning errors separately. Measure first, then decide whether changes are warranted. This baseline is planned, not a published result.
2. **VoiceBridge: independent setup feedback.** Review fresh full-host installation reports in the [beta ledger](https://github.com/nexora-studio-tr/voicebridge/blob/main/docs/BETA-STATUS.md). The initial learning target is two volunteers; no reviewed independent installation is claimed yet. A recorded demo alone does not qualify. [Join the beta](https://github.com/nexora-studio-tr/voicebridge/issues/1).
3. **ProofGate: architecture before workspace execution.** Design a narrow npm-workspace/Vitest path with source, package, policy and evidence identity. Implement only after scope review. Current execution remains single-package.
4. **Maintenance:** all six approved Actions updates are merged, with successful main CI linked in the [dependency record](MAINTENANCE.md). The record includes the Windows Node patch selection and CI retries. Two Node 26 type upgrades remain unmerged; any runtime/type support change requires a separate approved packet.

The other four products remain in maintenance during the VoiceBridge packet. Live Discord testing stays with the owner and does not block engineering or architecture work. Both language directions, overlapping speech, private playback and consent cancellation still need separate two-human acceptance. New product scopes and major architecture changes require a separate decision under the [governance guide](GOVERNANCE.md).

Installation checks and per-caption stage timings help diagnosis; neither proves speech quality, end-to-end listening latency or capacity. There is no delivery-date, tester-count or star-growth guarantee.

Each release includes meaningful automated checks, source/release identity, installation instructions and English/Turkish documentation. Independent human acceptance and deferred live tests are identified separately. Reproducible user feedback determines the next implementation priority.
