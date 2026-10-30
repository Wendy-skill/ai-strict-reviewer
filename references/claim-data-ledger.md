# Claim–Data Ledger | 共享命题与数据账本模板

## Purpose

Store *the identity and provenance* of recurring scientific statements, datasets, conditions, figures and versions so Reviewer and Quality Inspector need not independently extract the same inputs. This file is a **template**, not a live database and not automatic persistence.

## Header

- Project / manuscript: `[title or ID]`
- Manuscript version and date: `[exact]`
- Ledger version and custodian: `[version; author/user]`
- Evidence actually inspected: `[paths, papers, logs, tables, checks]`
- Evidence still missing: `[specific]`
- Last cross-member handoff: `[issue IDs]`

## Core claims (one statement per row)

| Claim ID | Claim (exact wording/meaning) | RQ/Objective | Source location | Figure/Table/Equation | Scope/conditions | Evidence status | Review status | Version |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| C-001 | `[literal, not invented]` | `RQ1` | `§X.Y` | `Fig. X` | `[which cases]` | Documented | Unverified | `v#` |

## Data and computation records

| Data ID | Metric and definition | Value / unit | Case / sample / time | Input dataset | Script/formula + tool | Figure/Table | Verification and limitations | Version |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| D-001 | `[definition]` | `[reported]` | `[condition]` | `[path]` | `[not yet checked]` | `Table X` | Reported; not recomputed | `v#` |

## Workflow / issue tracking

| Issue ID | Owner | Affected claim/data ID | Problem & evidence | Impact or severity | Required check/decision | State | Checked version |
| --- | --- | --- | --- | --- | --- | --- | --- |
| RG-001 | Reviewer | C-001 | `[refer to located evidence]` | `[local rubric]` | `[next action]` | Open | `v#` |

## Update rules

- A claim and a dataset can have different versions. Never overwrite the old source-of-truth record without recording the change.
- Preserve units, baselines, scope, sample sizes, particle/case definitions and uncertainty where relevant.
- A later value is not automatically more correct. Document why a value was superseded (new raw data, corrected formula, changed condition, approved analysis revision).
- Do not label data independently verified without a traceable calculation, image/source check or documented external confirmation.
- If source truth is undecidable, keep both candidates with `Needs verification` and assign the author a decision.
- Use stable identifiers across manuscript, figure, analysis script and issue list. If an earlier ID changes meaning, create a new ID and cross-reference it.
- For long documents process chapters in batches, summarise ledger entries, then audit Abstract–Results–Conclusions across all relevant versions.

## Handoff rule

Pass *only the relevant rows* + source locators and a version marker. Do not indiscriminately paste an entire long manuscript or rerun all already checked tasks.
