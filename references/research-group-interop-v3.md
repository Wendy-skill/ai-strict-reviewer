# v3 — Interface with the 17 Research Skills

This file is optional and never a claim that other agents, tools or accounts are connected. Read only for a real handoff.

## Ownership and scope

- **Member:** ai-strict-reviewer.
- **Own:** Scientific defensibility: methods, evidence, statistics and interpretation.
- **Optional specialists:** engineering-experiment-reviewer, engineering-review-paper-reviewer, simulation-paper-auditor, claim-evidence-checker and physics-sanity-check only for scoped questions.
- **Chinese triggers:** 严格审稿、科学性核查、方法与证据审查.
- **English triggers:** strict scientific review, evidence adequacy.
- **Do not activate for:** Formatting-only, pure language editing or final mechanical QA.

## Exact coordination contract

First load member-specific `coordination-protocol.md` and `specialist-routing.md` here. Transfer one row per root issue: `ID | owner | document/version/location | claim or issue | located evidence | source status | assessment | local Severity/Impact | next action | author decision | workflow state`.

Source status: `Reported / Documented / Independently checked / Not available`. Assessment: `Confirmed / Reasoned inference / Unverified`, with the exact object being verified. Workflow: `Open / Waiting for evidence / Awaiting author / Resolved / Recheck needed`. Reviewer **Severity** is scientific; Inspector **Impact** is document QA. Never force them onto one scale.

Reuse the supplied or explicitly created Claim/Data Ledger, respecting claim, data, calculation and manuscript versions; no automatic cross-app storage. One owner per issue. Only invoke other specialists when installed/accessible and appropriate. If the specialist or required source is absent, keep the work pending; do not claim delegation. After approved substantive changes, recheck affected claims and records, not the entire pipeline.
