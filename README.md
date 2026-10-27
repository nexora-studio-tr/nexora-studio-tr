<p align="center">
  <img src="https://raw.githubusercontent.com/nexora-studio-tr/nexora-studio-tr/main/assets/header.webp" alt="Nexora" width="100%" />
</p>

[English](README.md) · [Türkçe](README.tr.md) · [Product roadmap](ROADMAP.md)

I build open-source tools for problems that are easy to overlook: a conversation lost in translation, a test that proves too little, an access grant that never ends.

The work spans **developer tooling, Discord infrastructure and performance measurement**. Each project includes English/Turkish documentation, setup instructions and explicit validation limits.

## Selected work

| Project | The problem it tackles | Start here |
| :--- | :--- | :--- |
| **[VoiceBridge](https://github.com/nexora-studio-tr/voicebridge)** | Personal Turkish ↔ English captions and speech for Discord. Local models, per-speaker consent and private listening. | [alpha.3 / beta](https://github.com/nexora-studio-tr/voicebridge/releases/tag/v0.1.0-alpha.3) |
| **[ProofGate](https://github.com/nexora-studio-tr/proofgate)** | Check whether a test distinguishes a code change from its broken baseline, with bounded mutation evidence and CLI/MCP integration. | [Read-only demo](https://proofgate-demo.onrender.com/) |
| **[ReproPack](https://github.com/nexora-studio-tr/repropack)** | Reduce failing HTTP/PostgreSQL scenarios to smaller, verified reproductions while preserving the failure signature. | [Interactive demo](https://repropack-demo-4rq9.onrender.com/) |
| **[AccessLease](https://github.com/nexora-studio-tr/accesslease)** | Give temporary Discord access an independent approval, a permission preview and a verified expiry. | [alpha.1 / setup](https://github.com/nexora-studio-tr/accesslease/releases/tag/v0.1.0-alpha.1) |
| **[Nexora FrameLab](https://github.com/nexora-studio-tr/nexora-framelab)** | Discover Windows hardware, inspect CS2 frame times and evaluate recoverable settings experiments. | [Experimental Windows alpha](https://github.com/nexora-studio-tr/nexora-framelab/releases/tag/v0.1.0-alpha.1) |

**Release scope:** these projects are early releases. VoiceBridge is seeking multi-user beta feedback; AccessLease's live Discord acceptance test is pending. FrameLab has no live CS2 benchmark or demonstrated FPS gain. Demo data and execution limits are identified in each repository.

## How I build

- **Keep control local.** Self-hosted runtimes, documented configuration and explicit processing choices.
- **Make results inspectable.** Architecture notes, security policies, meaningful tests and validation records alongside the code.
- **Make recovery part of the design.** Consent revocation, bounded access, reproducible failures and reversible configuration changes where they apply.

**Main tools:** TypeScript · Python · Rust · PostgreSQL · React · Tauri

## Help shape the next release

VoiceBridge is the current beta focus. Try it with a second person and report recognition errors, consent behavior or listening latency in the **[beta thread →](https://github.com/nexora-studio-tr/voicebridge/issues/1)**. Please omit private conversations, credentials and server identifiers.

For other projects, use their issue forms and contribution guides. Report vulnerabilities through the affected repository's `SECURITY.md`.
