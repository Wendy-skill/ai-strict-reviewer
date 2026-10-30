# Cross-member coordination protocol

This reference describes **data exchange and optional delegation**, not an automatic multi-agent system. A role name does not mean a real subagent, specialised Skill, software program, or connector was invoked.

## 1. Entry and ownership

1. First honour the explicit user task. If only one member is installed, complete what that member can safely do and mark other work as pending.
2. Decide whether the issue needs a specialist. Use a specialist only when it is both **available** and **materially useful**. Do not recursively call the same underlying Skill through multiple members.
3. Assign one owner to each issue. A second role can provide a cross-check, not an independent duplicate full review.
4. Reuse a prior verified finding/ledger record if the document version, conditions and source remain the same. Reopen when evidence or versions changed.
5. Do not assert delegation or file persistence until tools confirm it happened. Give the user a self-contained follow-up task if no handoff tool is present.

## 2. Default flow with feedback

Literature → approved Research Execution → **scientific review** → language/structure editing → document Quality Inspection.

- This is a *default*, not a compulsory ordering. Basic structure editing may happen earlier.
- When the Reviewer finds inadequate evidence, send the issue back to Literature or Execution; never polish an unsupported claim into certainty.
- When the Inspector finds numerical/source-of-truth conflict, send it to the author or Execution; return science-affecting interpretation to Reviewer and meaning-affecting wording to Editor.
- Following a substantive change, rerun the **affected** reviews and QA checks, not the entire pipeline automatically.

## 3. Common issue / handoff record

Use these mandatory fields when transferring a finding; ordinary prose is fine for trivial requests:

| Field | Meaning |
| --- | --- |
| ID | Stable `RG-001`, `RG-002`... within a project; reuse ID for the same root issue |
| Owner / route | Current responsible member or specialist; planned and actually invoked are distinct |
| Location | File name, version, section, page, figure/table, or case ID |
| Issue | One falsifiable problem statement |
| Evidence | Direct excerpt/result + source locator; no invented verification |
| Source status | `Reported`, `Documented`, `Independently checked`, `Not available` |
| Assessment | `Confirmed`, `Reasoned inference`, `Unverified`; note what exactly is confirmed |
| Consequence | Use local rubric: Reviewer = scientific **Severity**; Inspector = document **Impact**; other roles = `Follow-up urgency` where useful; never map them into one false score |
| Proposed action | Specific check, revision, execution or source needed |
| Human decision | `Required` / `Not required` with reason if required |
| Workflow state | `Open`, `Waiting for evidence`, `Awaiting author`, `Resolved`, `Recheck needed` |

A record may be `Confirmed` as an internal **inconsistency** without proving which value is scientifically correct. Preserve member-specific status labels where they are more precise; the common fields are an exchange wrapper, not a replacement for detailed review vocabulary.

## 4. Evidence semantics

- `Reported`: manuscript / abstract / tool output asserts it; not independently verified.
- `Documented`: actual figure, table, method, source file, log or paper available to inspect.
- `Independently checked`: independently cross-checked/calculated/verified by an available tool, with trace.
- `Not available`: the needed material is missing/unreadable/inaccessible.
- `Confirmed`: precisely define what was confirmed (e.g. 'the paper contains this claim', **not** 'the underlying experiment is true').
- `Reasoned inference`: supported interpretation but not directly demonstrated.
- `Unverified`: source or calculation unavailable, or conflict unresolved.

## 5. Shared ledger usage

See `references/claim-data-ledger.md` for the canonical **schema**. The ledger is an *actual user-supplied or produced file*, not assumed shared memory. If one is supplied, read and reuse it; otherwise create a **provisional table in the current task**. Persist or update files only where tools and permissions permit and the user requests/authorises saving. Always annotate document version, raw/derived data provenance, conditions and verification status.

## 6. Compact handoff example

`RG-014 | Manuscript v6, Fig. 5 and §7.2 | Result quoted as 43% versus 38% | Documented | Confirmed mismatch; correct value Unverified | Impact: High | Author/Execution | Check calculation against versioned data; no auto-fix | Awaiting author`

## 7. When to load

Load this reference when coordinating with another member, exporting/importing issues, reviewing a prior audit, or preparing a shared research record. Do not read it again for each new sentence or trivial copy edit.
