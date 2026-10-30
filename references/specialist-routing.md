# Optional specialist routing — Strict Reviewer

## Activation

Trigger on 严格审稿 / 科学性 / 方法学 / 证据充分性 / 统计解释, or scientific review / methodology / evidence adequacy. Avoid activating for language-only editing or a pure format check.

## Task → optional Skill

| Scientific question | Optional specialist | Clear division of labour |
| --- | --- | --- |
| Engineering experimental design, measurement and uncertainty | `engineering-experiment-reviewer` | Return experiment-specific evidence/risk; Strict Reviewer owns final synthesis |
| Simulation credibility, mesh/time-step independence and V&V | `simulation-paper-auditor` | Return numerical-method audit; no second full review of same issue |
| Engineering literature review methodology and synthesis coverage | `engineering-review-paper-reviewer` | Review-specific evidence and scope, not generic manuscript rewriting |
| Claim versus source/figure evidence traceability | `claim-evidence-checker` | **Map the exact claim-evidence relationship** and unsupported leaps; scientific adequacy and severity belong to Strict Reviewer |
| Physical plausibility of model trends/mechanisms | `physics-sanity-check` | **Physical plausibility only**, not proof; do not infer mechanism as established from plausible trends |
| Target-journal fit comparison | `journal-gap-analyzer` | Separate comparative journal fit from scientific validity; avoid acceptance predictions |

## Routing and deduplication

- Route by *material question and evidence*, not by a fixed chain of all specialists.
- Use one primary reviewer per issue; parallel specialisms only for distinct questions or real cross-validation needs.
- Import specialist evidence with source locator, status and version, and assign scientific Severity only after synthesis.
- A Quality Inspector may report a factual figure-text mismatch, but science-consequential interpretation remains here.
- Literature Member verifies source existence/metadata; this Reviewer evaluates whether accessible evidence supports a claim.
- When the specialist is absent, do the supported baseline review under this Skill; report unverified dimensions, not fabricated delegation.
