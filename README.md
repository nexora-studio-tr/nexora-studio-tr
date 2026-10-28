<p align="center">
  <img src="https://raw.githubusercontent.com/nexora-studio-tr/nexora-studio-tr/main/assets/header.webp" alt="Nexora" width="100%" />
</p>

[English](README.md) · [Türkçe](README.tr.md) · [Roadmap](ROADMAP.md) · [Brand](BRAND.md) · [Governance](GOVERNANCE.md)

**Local control. Verifiable results.**

I build open-source tools for problems that are easy to overlook: a conversation lost in translation, a test that proves too little, an access grant that never ends.

The work spans **developer tooling, Discord infrastructure and performance measurement**. Each project includes English/Turkish documentation, setup instructions, automated tests and explicit validation limits.

## In focus: VoiceBridge

Read and hear a Discord conversation in your own language, with local processing and each speaker's consent. Turkish ↔ English is the current language pair; translated audio plays privately in your browser.

**[Download alpha.7 →](https://github.com/nexora-studio-tr/voicebridge/releases/tag/v0.1.0-alpha.7)** · **[Try the recorded demo →](https://github.com/nexora-studio-tr/voicebridge#recorded-demo)** · **[Host a beta installation →](https://github.com/nexora-studio-tr/voicebridge/blob/main/docs/BETA.md)**

The next engineering step is a repeatable Turkish/English quality baseline. In parallel, the beta milestone is **two reviewed independent fresh installations**. Two-person live acceptance remains with the owner and is recorded separately. [Follow the evidence](https://github.com/nexora-studio-tr/voicebridge/blob/main/docs/BETA-STATUS.md) or [share a test report](https://github.com/nexora-studio-tr/voicebridge/issues/new?template=beta_feedback.yml).

## Selected work

| Project                                                                    | Latest useful increment                                                                                                                                         | Release                                                                                                    |
| :------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------- |
| **[VoiceBridge](https://github.com/nexora-studio-tr/voicebridge)**         | Personal Turkish ↔ English captions and speech for Discord. Windows launcher, safe room recovery and an operator performance view with private numeric reports. | [0.1.0-alpha.7](https://github.com/nexora-studio-tr/voicebridge/releases/tag/v0.1.0-alpha.7)               |
| **[ProofGate](https://github.com/nexora-studio-tr/proofgate)**             | Test evidence for a code change, plus read-only workspace impact preflight with dependency reasons. Execution remains limited to a single npm package.          | [0.1.0-alpha.2](https://github.com/nexora-studio-tr/proofgate/releases/tag/v0.1.0-alpha.2)                 |
| **[ReproPack](https://github.com/nexora-studio-tr/repropack)**             | Smaller HTTP/PostgreSQL reproductions with deletion witnesses explaining the checks behind retained steps and partial evidence.                                 | [0.6.0-alpha.2](https://github.com/nexora-studio-tr/repropack/releases/tag/v0.6.0-alpha.2)                 |
| **[AccessLease](https://github.com/nexora-studio-tr/accesslease)**         | Temporary Discord access with independent review, verified expiry and linked renewal requests that preserve the original deadline while pending.                | [0.1.0-alpha.2](https://github.com/nexora-studio-tr/accesslease/releases/tag/v0.1.0-alpha.2)               |
| **[Nexora FrameLab](https://github.com/nexora-studio-tr/nexora-framelab)** | Windows hardware discovery and PresentMon capture comparison. Quality gates separate observed differences from incompatible measurements.                       | [0.1.0-alpha.2 · Windows](https://github.com/nexora-studio-tr/nexora-framelab/releases/tag/v0.1.0-alpha.2) |

**Release scope:** these are alpha releases with validation records and checksums. VoiceBridge still needs independent multi-user beta feedback; AccessLease's live Discord acceptance test is pending. FrameLab has no live CS2 benchmark or demonstrated FPS gain. Imported capture comparisons cannot apply settings.

Explore the synthetic **[ProofGate demo](https://proofgate-demo.onrender.com/)** and **[ReproPack demo](https://repropack-demo-4rq9.onrender.com/)**, or follow each tagged release's setup instructions.

## How I build

- **Keep control local.** Self-hosted runtimes, documented configuration and explicit processing choices.
- **Make results inspectable.** Architecture notes, security policies, meaningful tests and validation records alongside the code.
- **Make recovery part of the design.** Consent revocation, bounded access, reproducible failures and reversible configuration changes where they apply.

**Main tools:** TypeScript · Python · Rust · PostgreSQL · React · Tauri

## Help shape the next release

VoiceBridge is the current beta focus. Fresh installation feedback is useful even before a second person joins. Report setup friction, recognition errors, consent behavior or listening delay in the **[beta thread →](https://github.com/nexora-studio-tr/voicebridge/issues/1)**. Please omit private conversations, credentials and server identifiers.

For other projects, use their issue forms and contribution guides. Report vulnerabilities through the affected repository's `SECURITY.md`.

[Dependency review](MAINTENANCE.md) records the next maintenance decisions and their CI evidence.
