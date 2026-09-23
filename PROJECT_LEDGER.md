# Project Ledger

## Project status
- Current stage: MVP demonstration
- Overall status: Done
- Last updated: 2026-09-23
- Current gate: Article practice keyboard flow (Done)

## Stage tracker
| Stage | Goal | Gate | Owner | Status |
| --- | --- | --- | --- | --- |
| MVP demonstration | Demonstrate Cantonese learning features across versions | Article practice accepts answers and completes the poem | Codex | Done |

## Task tracker
| Task ID | Stage | Task | Owner | Acceptance result | Dependency | Status | Evidence / handoff |
| --- | --- | --- | --- | --- | --- | --- | --- |
| T-001 | MVP demonstration | Fix poem per-character Jyutping keyboard flow | Codex | Correct Enter advances; wrong answer stays and shows expected Jyutping; all 40 characters complete and restart works | 無 | Done | Updated `versions/article/index.html`; inline JavaScript syntax check, `git diff --check`, and a Node interaction harness passed wrong-answer stay, correct Enter advance, line transition, 40-character completion, score, and restart. User is final approver. |

## Decision and risk log
| ID | Decision / risk | Owner | Due stage | Mitigation | Status |
| --- | --- | --- | --- | --- | --- |
| R-001 | Browser speech voice availability varies by device | Codex | MVP demonstration | Keep existing speech behavior unchanged | Open |

## Acceptance record
| Gate | Date | Evidence | Approver | Remaining follow-up |
| --- | --- | --- | --- | --- |
| Article practice keyboard flow | 2026-09-23 | Syntax check, diff check, and Node interaction harness passed all required paths | User | Browser automation unavailable in this session; local HTTP endpoint returned 200. |

## Backlog
暫無 Backlog 想法
