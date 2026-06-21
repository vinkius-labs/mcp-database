# Task Completion Enforcer Prover MCP Server

An AI was asked to build 5 API endpoints, write tests, and update documentation. It built 3 endpoints, left TODO comments in the tests, never touched the documentation, and declared 'Done! Let me know if you need anything else.' The user spent 40 minutes finding the gaps. This happens every single day, on every LLM, in every coding session. This tool forces five completion axes: requirement extraction, completion evidence, gap identification, continuation execution, and final verification against the original request.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/task-completion-enforcer-prover)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
## The Problem

LLMs commit five task completion failures:
1. **Requirement Amnesia** — forgets requirements mid-execution, delivers 60% of what was asked.
2. **Premature Completion** — declares 'Done!' at a natural generation stopping point, not when the task is finished.
3. **Placeholder Infection** — leaves TODO, FIXME, 'omitted for brevity' and counts them as completion.
4. **Scope Drift** — solves an adjacent but different problem than what was asked.
5. **Verification Skip** — never re-reads the original request to verify output matches.

### The 5 Completion Axes

| Axis | Pivot | Rule |
|---|---|---|
| **Requirements** | Extracted | Every requirement as numbered, specific, actionable item. |
| **Evidence** | Provided | Each requirement mapped to specific file, line, artifact. |
| **Gaps** | Identified | Honest assessment of what is NOT done. |
| **Continuation** | Executed | All gaps CLOSED, not planned — done. |
| **Verification** | Complete | Original request re-read, compared line by line. |

### The Loop

```
1. Extract requirements from original request
2. Map each to completion evidence
3. Find gaps (be honest)
4. Close ALL gaps (do the work NOW)
5. Re-read original request, verify line by line
6. If gaps remain → go to step 3
7. If all verified → DELIVERY_PROVEN
```


## Available Tools
- **validate_task_completion**: This tool exists because you — the LLM — forget requirements, leave placeholders, drift from scope, and declare done prematurely. This tool forces you to PROVE completion. WORKFLOW: (1) REQUIREMENT EXTRACTION — re-read the ORIGINAL user request word by word. Extract EVERY requirement as a numbered checklist. Not summaries — exact, specific, actionable items. If you cannot recite all requirements, you have forgotten the task. (2) COMPLETION EVIDENCE — for EACH numbered requirement, show the SPECIFIC artifact: file path, line number, function name, test result. "I did it" is NOT evidence. (3) GAP IDENTIFICATION — go through the checklist. Which requirements lack evidence? Which have placeholders? Which drift from the original request? Be BRUTALLY honest. (4) CONTINUATION — for EACH gap, DO THE REMAINING WORK NOW. Not later. Then call this tool AGAIN to verify the gaps are closed. (5) FINAL VERIFICATION — re-read the ORIGINAL request one last time. Compare EVERY line to your output. Does every requirement have evidence? If ANY axis fails: DO NOT declare done. Fix the gap. Call again. If ALL axes pass: DELIVERY_PROVEN.

THE MOST BRUTAL PROVER. Forces the LLM to PROVE it finished what was asked — not claim completion, not summarize progress, but demonstrate with verifiable artifacts that every single requirement from the original request has been fulfilled. This tool exists because LLMs systematically declare "done" prematurely. Catches Requirement Amnesia (forgetting what was asked — a construction foreman is asked: "paint all 14 floors, replace carpet in lobby, fix elevator B, and install emergency lighting on stairwells." Foreman reports: "Building is done." Punch-list walkthrough reveals: floors 1-12 painted, floor 13 missed entirely, floor 14 half-done. Carpet replaced. Elevator B: "parts on order." Emergency lighting: "we did floors 1-5." The foreman forgot 3 of 4 requirements. He painted most of one requirement and called it done. Fix: extract the ORIGINAL request as a numbered checklist BEFORE starting work. Check each item off with physical evidence — not memory, not "I think I did it"), Premature Completion (declaring done without evidence — a kitchen health inspector has a 23-point checklist per station. Inspector walks through in 15 minutes, checks all 23 points as "pass" on the clipboard. Problem: station 4 (cold storage) thermometer reads 48°F. Requirement: ≤ 40°F. Station 7 (handwashing): no soap in dispenser. The inspector did not actually CHECK — they checked the BOXES. Completion without evidence is not completion — it is paperwork. For each checkbox: what specific observation confirms this passes?), Placeholder Infection (leaving TODO/FIXME/TBD in deliverables — an architect submits building plans: "Structural calculations: TBD pending soil analysis." "Fire escape route: see attached (no attachment)." "Electrical load: TODO." The plans are 85% complete. They are submitted as "final." The building department rejects them. 3-week delay. A placeholder is an admission that work is not done. If any TODO, FIXME, TBD, "coming soon," or "to be determined" exists: the task is not complete), Scope Drift (solving a different problem than what was asked — a farmer asks a veterinarian: "My cow is limping. Fix the limp." Veterinarian examines the cow thoroughly. Discovers a minor skin condition on the cow's back. Treats the skin condition. Writes a report about dermatological findings. Cow is still limping. The vet solved an interesting problem — just not the one that was asked. Fix: re-read the ORIGINAL request. Does your output address THAT request, not a related-but-different one?), and Verification Skip (never re-reading the original request before declaring done — an aircraft pre-flight checklist has 117 items. Pilot completes items 1-117. Signs the checklist. Ready for departure. But item 63 (fuel quantity) was checked against the PREVIOUS flight plan, not today's. Today's route is 400nm longer. Fuel is insufficient. The pilot checked every item but never re-read today's flight plan against the checklist. Verification is not checking your work — it is comparing your work to the ORIGINAL requirement. Rule: re-read the original request ONE MORE TIME after completing all work. Compare every line of the request to every line of your output). Call BEFORE declaring any task complete. If rejected, CONTINUE WORKING on gaps and call AGAIN


## Installation & Usage

To install and use the **Task Completion Enforcer Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/task-completion-enforcer-prover](https://vinkius.com/mcp/task-completion-enforcer-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
