# Dependency review — 27 October 2026

[Türkçe](MAINTENANCE.tr.md) · [Roadmap](ROADMAP.md) · [Governance](GOVERNANCE.md)

The initial read-only review covered eight open Dependabot PRs in ProofGate and ReproPack. The owner subsequently approved the two changes recorded below. The original review snapshot is retained for traceability; PR heads and CI may change. No verified vulnerability requiring an emergency upgrade was established by the initial review.

## Applied maintenance

The two approved changes were merged sequentially. Each link identifies the merge commit and its main-branch validation.

| Change                                                                                      | Merge commit                                                                                               | Main CI                                                                                                                    |
| :------------------------------------------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| [ProofGate #1](https://github.com/nexora-studio-tr/proofgate/pull/1): upload-artifact 7.0.2 | [`447891e`](https://github.com/nexora-studio-tr/proofgate/commit/447891e1581d408c1052ab7a0eb49543989cb05e) | [Windows, Ubuntu, browser and execution](https://github.com/nexora-studio-tr/proofgate/actions/runs/40574993962)           |
| [ReproPack #2](https://github.com/nexora-studio-tr/repropack/pull/2): checkout 7.0.1        | [`2ee039d`](https://github.com/nexora-studio-tr/repropack/commit/2ee039ddf2c5e4ca6e83e9cfa71075cf94310bce) | [Windows, Ubuntu, browser, sandbox and deployment](https://github.com/nexora-studio-tr/repropack/actions/runs/40575567120) |

ProofGate's two PR artifact ZIPs were downloaded and checked against GitHub's SHA-256 digests. They contain the expected Docker, isolation, integration, MCP, deployment and browser reports, with the expected screenshots; both artifact names were also checked on the merged main run. ReproPack retains full action pins and `persist-credentials: false`. Runtime versions and tagged release assets were unchanged. No release-tag publication was triggered; the release workflow's checkout change was reviewed in configuration.

The remaining four Actions PRs and two Node 26 type PRs were not modified by this maintenance packet. Their next actions require a separate approved scope and fresh evidence.

## Initial review snapshot

Compared against ProofGate main [`bd22f4b`](https://github.com/nexora-studio-tr/proofgate/commit/bd22f4ba2fec906d248261281ea6ee0b13e69473) and ReproPack main [`bc90cd0`](https://github.com/nexora-studio-tr/repropack/commit/bc90cd0616dce3b168bf3e75b9336a70bd132ed6). “Current base” refers to those commits. The CI links below ran on the identified PR head and its then-current merge base.

### Recommendations at review time

| PR                                                                   | Change                        | Reviewed head  | CI evidence                                                                                    | Next action                                                                                              |
| :------------------------------------------------------------------- | :---------------------------- | :------------- | :--------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------- |
| [ProofGate #1](https://github.com/nexora-studio-tr/proofgate/pull/1) | upload-artifact 6.0.0 → 7.0.2 | `dc2b2660ce6f` | [Passed; current base](https://github.com/nexora-studio-tr/proofgate/actions/runs/40459092122) | Candidate for an approved maintenance packet. Recheck head, CI and uploaded reports before merging.      |
| [ProofGate #2](https://github.com/nexora-studio-tr/proofgate/pull/2) | checkout 6.1.0 → 7.0.1        | `44507e7bbe1c` | [Failed; older base](https://github.com/nexora-studio-tr/proofgate/actions/runs/40169185035)   | Refresh onto current main, then rerun all checks. Windows formatting and Docker input access failed.     |
| [ProofGate #3](https://github.com/nexora-studio-tr/proofgate/pull/3) | setup-node 6.5.0 → 7.1.0      | `7820028e5acd` | [Failed; older base](https://github.com/nexora-studio-tr/proofgate/actions/runs/40169191229)   | Refresh and rerun. Keep the explicit project Node version; inspect cache/install behavior.               |
| [ProofGate #4](https://github.com/nexora-studio-tr/proofgate/pull/4) | @types/node 24.19.2 → 26.6.5  | `00f4f1677f46` | [Failed; older base](https://github.com/nexora-studio-tr/proofgate/actions/runs/40169198254)   | Hold the Node 26 type upgrade. Keep the declared Node 24 runtime/type line aligned.                      |
| [ReproPack #1](https://github.com/nexora-studio-tr/repropack/pull/1) | upload-artifact 4.6.2 → 7.0.2 | `251378dd269d` | [Failed; older base](https://github.com/nexora-studio-tr/repropack/actions/runs/40129423905)   | Refresh and rerun. Verify both artifact names and report/archive contents.                               |
| [ReproPack #2](https://github.com/nexora-studio-tr/repropack/pull/2) | checkout 6.1.0 → 7.0.1        | `8a3982d36575` | [Passed; current base](https://github.com/nexora-studio-tr/repropack/actions/runs/40506652126) | Candidate for an approved maintenance packet. Recheck exact head and CI before merging.                  |
| [ReproPack #3](https://github.com/nexora-studio-tr/repropack/pull/3) | setup-node 6.5.0 → 7.1.0      | `695bed64b95d` | [Failed; older base](https://github.com/nexora-studio-tr/repropack/actions/runs/40129438672)   | Refresh and rerun, including the Windows PostgreSQL wrapper and Linux checks.                            |
| [ReproPack #4](https://github.com/nexora-studio-tr/repropack/pull/4) | @types/node 24.19.2 → 26.6.5  | `d4d9ebf007c2` | [Failed; current base](https://github.com/nexora-studio-tr/repropack/actions/runs/40506695016) | Hold. Type checking fails in process guardians and identity tests; runtime support is tested on Node 24. |

## Compatibility and failure evidence

- **checkout v7:** upstream changes fork checkout behavior under privileged `pull_request_target` / `workflow_run` triggers. These repositories use ordinary `pull_request`, push and reusable workflows; no unsafe-checkout opt-in is proposed. Both PRs preserve `persist-credentials: false` and full commit pins. [Pinned upstream changes](https://github.com/actions/checkout/blob/3d3c42e5aac5ba805825da76410c181273ba90b1/README.md#checkout-v7).
- **setup-node v7:** removes the dummy `NODE_AUTH_TOKEN` fallback. The reviewed workflows do not set `registry-url` or use that fallback. They still explicitly request project Node **24.15.0**. The action's own Node 24 execution runtime is a separate concern; v7 does not select Node 26 for the project. [Pinned upstream changes](https://github.com/actions/setup-node/blob/949feb2413d6458794dcd2491c4babbbce0c15c1/README.md#whats-new-in-v7).
- **upload-artifact v7:** adds optional direct single-file uploads and ESM internals; the reviewed workflows do not request `archive: false`. Preserve existing report globs, artifact names and missing-file failures, and inspect downloadable contents after an update. This review covers GitHub.com hosted runners, not GHES or an arbitrary self-hosted runner. [v7 changes](https://github.com/actions/upload-artifact/releases/tag/v7.0.0), [v7.0.2 retry changes](https://github.com/actions/upload-artifact/releases/tag/v7.0.2).
- **Older ProofGate failures:** [Windows formatting](https://github.com/nexora-studio-tr/proofgate/actions/runs/40169185035/job/121096378285) reported 54 files; [Docker execution](https://github.com/nexora-studio-tr/proofgate/actions/runs/40169185035/job/121096378322) could not read `/input/input.json` (`EACCES`). The setup-node and type PRs show the same Docker symptom. These historical failures do not establish that the proposed action or type version caused them, or that a current-base rerun will pass.
- **Older ReproPack failures:** [upload-artifact PR Windows job](https://github.com/nexora-studio-tr/repropack/actions/runs/40129423905/job/120977755289) and [setup-node PR Windows job](https://github.com/nexora-studio-tr/repropack/actions/runs/40129438672/job/120977796570) failed because PostgreSQL refused an administrative Windows process. They predate the current Windows wrapper.
- **Current ReproPack type failure:** [Ubuntu typecheck](https://github.com/nexora-studio-tr/repropack/actions/runs/40506695016/job/122197697602) reports TS2722 in process guardians and TS2769 in identity tests. The PR also changes `undici-types` 7 → 8. Do not mask this by disabling strictness or claiming that new type declarations add runtime support.

## Remaining work

The two passing Actions candidates were handled in the approved packet above. The proposed next packet is to refresh the four older Actions branches against current main, inspect their new diffs and rerun their checks before any merge. Both Node 26 type PRs remain unmerged pending a deliberate runtime-support decision; staying on compatible Node 24 types is the proposed path. Recheck all evidence before action rather than treating this snapshot as permanent approval.
