# Product & engineering roadmap

[Türkçe](ROADMAP.tr.md) · [Profile](README.md)

Updated 27 October 2026. This is the development order, not a delivery-date or performance promise. One usable increment is completed before starting the next implementation.

| Priority | Product | Next meaningful outcome |
| :--- | :--- | :--- |
| **Current delivery** | **VoiceBridge** | [Alpha.3](https://github.com/nexora-studio-tr/voicebridge/releases/tag/v0.1.0-alpha.3): guided setup checks and a reviewed, private support report. [Implementation and checks](https://github.com/nexora-studio-tr/voicebridge/pull/2). |
| **Next architecture** | **ProofGate** | Design workspace-aware verification for npm monorepos: freeze the package/dependency graph, select affected tests and bind before/after evidence to each package. Current support remains a single npm package. |
| **Following research** | **ReproPack** | Design durable PostgreSQL replay state across restarts. Current snapshots are scoped to the running registry; a successful demo does not prove durable replay. |
| **Acceptance pending** | **AccessLease** | Exercise real grant, expiry, external role changes and restart recovery in a dedicated Discord test server. The live acceptance test remains deferred. |
| **Experimental** | **Nexora FrameLab** | Validate real CS2 replay/capture/recovery and collect results on named hardware before making tuning or FPS-gain claims. Live game testing remains deferred. |

## Current user-validation gate

VoiceBridge still needs an independent human installation and two distinct people testing both language directions, overlapping speech, personal playback and consent cancellation. Guided setup results are installation snapshots, not speech-quality or live-test evidence. [Join the beta](https://github.com/nexora-studio-tr/voicebridge/issues/1).

Each increment carries meaningful tests, repeatable installation, source/release identity and English/Turkish instructions. Architecture for the next substantial expansion is reviewed before implementation. Actual feedback and reproducible failures determine changes to this order.
