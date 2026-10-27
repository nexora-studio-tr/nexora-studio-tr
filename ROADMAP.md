# Product & engineering roadmap

[Türkçe](ROADMAP.tr.md) · [Profile](README.md)

Updated 27 October 2026. Five usable increments were delivered sequentially. The next gates below are validation and architecture work, without delivery-date or performance promises.

| Product             | Released increment                                                                                                                                                        | Next meaningful gate                                                                                                                                    |
| :------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **VoiceBridge**     | [Alpha.4](https://github.com/nexora-studio-tr/voicebridge/releases/tag/v0.1.0-alpha.4): queue-inclusive per-caption timings and bilingual stage explanations.             | Independent installation and two-person language, overlap, playback and consent tests. Timings exclude capture, Discord transport and browser playback. |
| **ProofGate**       | [Alpha.2](https://github.com/nexora-studio-tr/proofgate/releases/tag/v0.1.0-alpha.2): read-only workspace dependency impact preflight.                                    | Review package-bound execution/evidence architecture before implementing monorepo test execution. Current execution remains single-package npm/Vitest.  |
| **ReproPack**       | [0.6.0-alpha.2](https://github.com/nexora-studio-tr/repropack/releases/tag/v0.6.0-alpha.2): retained-step deletion witnesses and explicit partial certification evidence. | Durable PostgreSQL replay across registry restarts and an independent pilot. Current snapshot lifetime remains registry-bound.                          |
| **AccessLease**     | [Alpha.2](https://github.com/nexora-studio-tr/accesslease/releases/tag/v0.1.0-alpha.2): linked renewals requiring independent approval, with unchanged original expiry.   | Dedicated live Discord grant, expiry, administrator intervention and restart acceptance. This test remains deferred.                                    |
| **Nexora FrameLab** | [Alpha.2](https://github.com/nexora-studio-tr/nexora-framelab/releases/tag/v0.1.0-alpha.2): observational comparison of imported captures with explicit quality gates.    | Live CS2 replay/capture/recovery and named-hardware measurements before any tuning or FPS-gain claim. Live game testing remains deferred.               |

## Current focus and sequence

1. **VoiceBridge: two independent fresh installations.** Invite volunteers, review their setup reports and record accepted evidence in the [beta ledger](https://github.com/nexora-studio-tr/voicebridge/blob/main/docs/BETA-STATUS.md). A recorded demo run alone does not qualify. No reviewed independent installation is claimed yet.
2. **VoiceBridge: two distinct humans in a live room.** Test both language directions, overlapping speech, private playback and consent cancellation. This remains separate from installation success. [Join the beta](https://github.com/nexora-studio-tr/voicebridge/issues/1).
3. **Maintenance:** all six approved Actions updates are merged, with successful main CI linked in the [dependency record](MAINTENANCE.md). The record includes the Windows Node patch selection and CI retries. Two Node 26 type upgrades remain unmerged; any runtime/type support change requires a separate approved packet.

The other four products remain in maintenance while this feedback is collected. New product scopes and major architecture changes require a separate decision under the [governance guide](GOVERNANCE.md).

Installation checks and per-caption stage timings help diagnosis; neither proves speech quality, end-to-end listening latency or capacity. There is no delivery-date, tester-count or star-growth guarantee.

Each release includes meaningful automated checks, source/release identity, installation instructions and English/Turkish documentation. Independent human acceptance and deferred live tests are identified separately. Reproducible user feedback determines the next implementation priority.
