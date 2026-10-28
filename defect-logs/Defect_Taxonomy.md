# Task 2 — Defect Taxonomy

## Scope

This taxonomy supports review of the supplied PSVS requirements S1–S12. A defect may receive one primary category in the log; a requirement can have several separate defects. Severity is a review priority, not a quantified probability or safety classification.

| Category | Definition | Example from this specification | Typical evidence/test |
|---|---|---|---|
| Ambiguity | Wording has two or more materially different reasonable interpretations. | S10 “per year” could mean calendar year, rolling 365 days, or another period. | Ask two reviewers to interpret the same case; differing decisions show ambiguity. |
| Vagueness | A term lacks a measurable boundary or operational meaning. | S2 “a large number”; S12 “good audit trail.” | Attempt to derive a pass/fail test; no threshold or criterion exists. |
| Incompleteness | Necessary actors, conditions, exceptions, data, or outcomes are omitted. | S1 does not say who registers depositors or what registration status is checked. | Enumerate boundary cases and required decisions; identify unspecified branches. |
| Contradiction | Two requirements prescribe incompatible behavior for the same conditions, without a precedence rule. | S7 caps temperature at -18°C while S8 permits warming to 0°C during maintenance. | Construct one state in which both rules apply; check whether both can be satisfied. |
| Non-verifiability | The statement lacks observable/measurable acceptance criteria or a defined observation method. | S9 says “promptly” but supplies no deadline, flag state, or test oracle. | Attempt to design a repeatable test with inputs, clock, and pass/fail result. |
| Redundancy / overlap | Requirements restate overlapping obligation without clarifying whether one adds a distinct constraint. | S6 “safe temperature” overlaps partly with S7’s temperature ceiling, but does not define a separate range. | Compare scopes and show whether each requirement can be independently satisfied or violated. |
| Infeasibility / potential infeasibility | A requirement may be impossible to meet under physical, operational, or stated exceptional conditions. | A literal absolute S7 “never above -18°C” may be physically incompatible with S8 maintenance warming to 0°C. | Consider actuator/sensor limits and explicit exceptions; confirm with engineering evidence before treating as proven infeasible. |
| Untraceability | The requirement lacks a clear source, owner, rationale, identifier relationship, or verifiable link to downstream evidence. | S12 requires a “good audit trail” but specifies no event fields or evidence linking actions to actors. | Try to map required evidence to the statement and its verification record. |

## Severity scale

| Severity | Meaning for this review |
|---|---|
| High | Could authorize unsafe, unauthorized, or conservation-damaging behavior, or contains a direct conflict affecting a critical control. |
| Medium | Affects core correctness or makes acceptance/recovery decisions unreliable; no immediate direct hazard established by the supplied text alone. |
| Low | Primarily a documentation, consistency, or future-maintenance concern; still needs disposition before final specification approval. |

## Classification note

The categories describe specification quality. “Potential infeasibility” is deliberately provisional: no physical design data was supplied. The Task 2 log records evidence and proposed resolution questions; it does not silently amend the baseline.
