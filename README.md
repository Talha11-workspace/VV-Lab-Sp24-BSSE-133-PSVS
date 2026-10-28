# PSVS Verification and Validation Lab

Repository: VV-Lab-Sp24-BSSE-133-PSVS  
Student: Talha Khalil  
System under study: Polar Seed Vault System (PSVS)

## Scope

Only Task 1 (orientation and configuration management) and Task 2 (defect taxonomy and verification logging) are being completed now. Tasks 3–7 remain pending.

## Task 1–2 artifacts

- [PSVS-REQ-v1.0 baseline](requirements/PSVS-REQ-v1.0.md) — supplied S1–S12 committed as PSVS-REQ-v1.0 and tagged baseline-1.
- [Change request template](change-request-template.md) — ID, artifact, reason, impact, and approver fields.
- [Defect taxonomy](defect-logs/Defect_Taxonomy.md) — eight required categories with definitions and examples.
- [Defect log](defect-logs/Defect_Log.md) — 23 findings against S1–S12, including cross-requirement issues.
- [Peer comparison](defect-logs/Peer_Review_Comparison.md) — simulated independent second pass only; not Abdullah Siddiqui’s actual authored log.
- [Defect summary](defect-logs/Defect_Summary.md) and [chart](defect-logs/Defect_Summary_Chart.svg) — category and severity counts.

## Required folders

requirements/ · defect-logs/ · abstractions/ · models/ · operations/ · constraints/ · proofs/ · reports/

## Configuration management

The S1–S12 baseline is immutable at tag baseline-1. Task 2 analysis is developed on defect-analysis and merged into main in a pull request. See commit history and repository graph for the staged changes.

## Limitations and status

The requirements contain unresolved ambiguities and contradictions; this work records them without silently changing the baseline. The classmate comparison is a clearly labeled simulated proxy based on S1–S12 because no actual peer log was provided. Its 82.6% detection rate is illustrative only and is not a measured peer-exchange result.

Tasks 3–7 are pending. This is an educational analysis, not a formal safety case for a real seed vault.
