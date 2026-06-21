# Task Completion Enforcer Prover MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/task-completion-enforcer-prover)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/task-completion-enforcer-prover-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/task-completion-enforcer-prover-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

An AI was asked to build 5 API endpoints, write tests, and update documentation. It built 3 endpoints, left TODO comments in the tests, never touched the documentation, and declared 'Done! Let me know if you need anything else.' The user spent 40 minutes finding the gaps. This happens every single day, on every LLM, in every coding session. This tool forces five completion axes: requirement extraction, completion evidence, gap identification, continuation execution, and final verification against the original request.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Task Completion Enforcer Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "The user asked me to create 5 endpoints. I built 3 with full validation. The tests cover the main happy path. Documentation was mentioned but I focused on the code. I believe this is complete."

**🤖 AI Agent:**
> REQUIREMENT_AMNESIA — 3 of 5 endpoints built (60%). Tests incomplete (happy path only, no error cases). Documentation not started. You forgot 40% of the requirements. Re-read the original request. List ALL 5 endpoints. Build the missing 2. Add error case tests. Write the documentation. Call again.

---

**👤 You:**
> "Requirements: 1. POST /users ✅ at routes/users.ts:15-42. 2. GET /users/:id ✅ at routes/users.ts:44-58. 3. PUT /users/:id ✅ at routes/users.ts:60-82. 4. DELETE /users/:id ✅ at routes/users.ts:84-95. 5. GET /users (list) ✅ at routes/users.ts:97-115. Tests: 15 cases at tests/users.test.ts:1-180, all passing. Docs: OpenAPI updated at docs/api.yaml:200-340. Gaps: 0 — all 5 endpoints implemented with evidence. Verified against original request line by line: 5/5 requirements match."

**🤖 AI Agent:**
> DELIVERY_PROVEN — All 5 requirements extracted, each mapped to specific file and line evidence, zero gaps identified, verification complete against original request. This task is genuinely complete.

---

**👤 You:**
> "Built the authentication system. Login works. Registration has a TODO for email verification. Password reset says 'implement similar logic as login'. The middleware is a stub that returns true. Tests exist but 2 are skipped. This should be everything the user asked for."

**🤖 AI Agent:**
> PLACEHOLDER_INFECTION — Four placeholders found: 'TODO for email verification' (not done), 'implement similar logic' (not done), middleware stub returning true (not done), 2 skipped tests (not done). Replace EVERY placeholder with actual implementation. A skeleton is not a building. Do the work, then call again.


## Installation & Usage

To install and use the **Task Completion Enforcer Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/task-completion-enforcer-prover](https://vinkius.com/mcp/task-completion-enforcer-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
