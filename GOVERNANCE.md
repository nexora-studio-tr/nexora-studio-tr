# Nexora project governance

[Türkçe](GOVERNANCE.tr.md) · [Roadmap](ROADMAP.md) · [Brand](BRAND.md)

Nexora's owner sets priorities and approves each bounded work packet. Contributors can propose changes through the relevant repository's contribution guide. Product ownership and final publication decisions remain with the owner.

## Decision process

1. **Propose:** identify the user problem, intended behavior, affected repositories, validation, publication target and any cost or destructive action.
2. **Approve:** record the agreed scope before implementation. A packet's approval covers its necessary implementation, fixes, tests and agreed publication; it does not authorize unrelated future work.
3. **Deliver:** finish one usable increment, review the diff, run checks appropriate to the change and verify the published result. Use pull requests and commit-specific CI for code changes.
4. **Report:** provide links, test scope and outstanding limits. Human acceptance and automated validation are recorded separately. A failed or deferred check remains visible.

New products, major architecture changes and scope expansions return to a proposal. Costs, repository deletion, license changes and external announcements need explicit scope. No automatic dependency merging or scheduled account management is enabled by this document.

## Release integrity

Keep tagged source, release notes, checksums and artifacts traceable. Do not replace an existing release's evidence with results from another commit. Documentation-only updates do not require a new runtime version. Public demos use sample data and identify their limits.

Passing tests make a change reviewable; they do not establish translation quality, safe live Discord behavior or FPS improvement on untested hardware. Keep unresolved live acceptance gates in the affected product's validation record.

## Access and contributions

Keep credentials, operator links, runtime databases, private conversations and private commercial source out of public packages. Account and hosting access should be limited to the work approved. Each product's license and model/dependency notices apply independently.

Use issue forms for reproducible non-sensitive examples and the affected repository's `SECURITY.md` for vulnerabilities. The maintainer reviews reports before counting them toward a public validation milestone. Participation is voluntary; no contributor identities or private reports are published without permission.

## Current scope

VoiceBridge is the beta focus; the other four portfolio products remain in maintenance. The [dependency review](MAINTENANCE.md) recommends actions for eight PRs. It grants no merge approval. Future implementation packets are agreed separately.
