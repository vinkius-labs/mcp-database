# Spec Prover MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/spec-prover)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/spec-prover-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/spec-prover-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Catch broken formulas before they reach your codebase. Spec Prover forces AI agents to prove every specification works with real inputs — one trace exposes bugs that abstract review never finds.

## Description
When an AI Product Manager writes a specification, it faces a critical blind spot: **formulas it has never traced with real inputs.** A PM writes `bedtime = wake_time - (cycles × 90 + 15)` without asking: what happens when the subtraction goes negative? What happens at midnight? Spec Prover eliminates this failure mode.

### The Problem It Solves

In multi-agent pipelines, the PM's specification is the first domino. A wrong formula cascades through every downstream agent:

- **Developer** implements the wrong formula faithfully
- **QA** writes tests against the wrong spec — tests pass because both are wrong
- **Publisher** ships a broken product to production

Or worse: QA accidentally writes correct expected values → tests fail → QA blames Developer → Developer can't fix (spec says otherwise) → **pipeline deadlock**.

### How It Works

Spec Prover uses three **Decision Pivots** — boolean checkpoints that the PM must commit to for every engine function:

1. **Trace** the formula step-by-step with concrete inputs (variable = expression = value).
2. **Verify output** — does the final traced value match the declared output?
3. **Check constants** — do ALL declared domain constants appear in the trace?
4. **Trace an edge case** — zero, negative, maximum, wrap-around.
5. **Check handling** — does the spec explicitly handle the boundary condition?

The tool **validates logical consistency** — if the PM says `SPEC_PROVEN` but `edgeCaseHandled: false`, the tool rejects with a clear explanation.

### Why It Works

- **One concrete trace catches more bugs than reviewing a formula abstractly.** The midnight crossover bug would have been caught by tracing `cycles=6, wake=08:00`.
- **Tool calls are obligations.** The PM cannot skip the proof step — it must fill every field before the spec reaches the developer.
- **Proactive, not reactive.** Unlike post-hoc testing, Spec Prover catches errors at the source — before they contaminate the entire pipeline.


## Available Tools
- **prove_spec_function**: You must execute a mathematical proof with concrete inputs: (1) CHOOSE a representative input — not a trivial case (0, 1) but a realistic value that exercises the main code path. Show EVERY intermediate step with arithmetic, (2) VERIFY output — does the final value in your trace match your expected output? If not: your formula has an error. The trace proves where the discrepancy starts, (3) CHECK constants — does EVERY declared constant appear in at least one step? If not: the constant is orphaned (spec is incomplete or noisy), (4) CHOOSE an edge case — boundary inputs that stress the formula: zero, negative, maximum, midnight wrap, empty array, single element. The edge case MUST differ from the representative input, (5) VERIFY edge case — does your spec explicitly handle the condition revealed? Does it define behavior for zero division? Negative results? Overflow? Wrap-around? If not: the spec is incomplete — the developer will guess, and guess wrong. If the tool rejects, re-examine your trace — your reasoning has a gap.

Structured proof tool — forces the PM agent to TRACE every formula with concrete inputs and verify edge cases BEFORE the spec reaches the developer. Based on ARTEMIS (2026), process reward models, and the mathematical proof methodology where every step must be independently verifiable. The tool validates logical consistency — if your verdict contradicts your own trace, it rejects. Catches Off-by-One Boundary (the most common arithmetic error in specifications — spec says: "Display the last 5 entries." Implementation: entries.slice(entries.length - 5). Input: 3 entries. entries.length - 5 = -2. slice(-2) returns last 2 entries — not an error, but unexpected. Input: 0 entries. entries.length - 5 = -5. slice(-5) on empty array = []. Correct by accident. Input: 5 entries. slice(0) = all 5. Correct. Input: 6 entries. slice(1) = last 5. Correct. But the spec never defined: what happens when entries < 5? Show all? Show empty? Show error? The developer guesses. The PM assumed. The QA tests with 10 entries. Production user has 2 entries and sees unexpected behavior. Fix: spec MUST define behavior for boundary inputs: 0 entries, 1 entry, exactly N, N+1), Floating-Point Precision Loss (arithmetic that loses precision in real computation — spec says: "Calculate 15% discount on $19.99." Trace: $19.99 × 0.15 = $2.9985. Rounded to cents: $3.00. Discounted price: $16.99. Implementation: 19.99 * 0.15 = 2.9984999999999995 (IEEE 754). Math.round(2.9984999999999995 * 100) / 100 = 3.00. OK — works here. But: $0.10 + $0.20 = 0.30000000000000004 in JavaScript. If the spec compares prices: if (total === expectedTotal) — fails. Fix: spec must define precision strategy: integer cents (1999 not 19.99), Decimal.js for arbitrary precision, or epsilon comparison (Math.abs(a-b) < 0.005). The trace must use ACTUAL floating-point arithmetic, not idealized math), Modular Arithmetic Wrap (time/circular calculations that wrap around boundaries — spec says: "Calculate bedtime: subtract sleep duration from wake time." wakeTime = 08:00 (480 minutes). sleepDuration = 9 hours (540 minutes). Trace: 480 - 540 = -60 minutes. What is -60 minutes? The spec does not say. Correct: (-60 + 1440) % 1440 = 1380 minutes = 23:00. But: what if the result is exactly 0? 0 = 00:00 or 24:00? Are they the same? What if sleepDuration > 24 hours? (480 - 1500 = -1020) → (-1020 + 1440) = 420 → 07:00. Is that correct? The spec MUST define the modular arithmetic explicitly and handle the wrap-around at midnight/boundaries), Undefined Division (division operations where the divisor can be zero — spec says: "Calculate average rating: sum of ratings / number of ratings." Normal case: ratings = [4, 5, 3, 4]. Sum = 16. Count = 4. Average = 4.0. Edge case: ratings = []. Sum = 0. Count = 0. Average = 0/0 = NaN. The spec NEVER addressed empty input. The developer implements sum/count. User with 0 reviews sees "NaN stars" displayed in the UI. Or worse: the NaN propagates through calculations: price × NaN = NaN. Fix: spec must define: "If no ratings exist, display 'No ratings yet' instead of average. Function returns null, not NaN. Caller handles null explicitly"), and Orphan Constants (declared constants that never appear in any formula — spec declares: CYCLE_DURATION_MIN = 90, FALL_ASLEEP_MIN = 15, REM_PHASE_MIN = 20. Formulas use: CYCLE_DURATION_MIN and FALL_ASLEEP_MIN. REM_PHASE_MIN is declared but never used in any step. This means either: (1) the spec forgot to include REM_PHASE_MIN in a formula (spec is incomplete), or (2) REM_PHASE_MIN is unnecessary (spec has dead constants — misleading). Both are errors. Every declared constant MUST appear in at least one formula step. If it does not: the spec has a gap or noise). Call once per engine function in the specification


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spec Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I wrote a spec for calculateBedtime(wakeTime, cycles). The formula is: totalMinutes = wakeHour×60 - (cycles×90 + 15). Prove this function works."

**🤖 AI Agent:**
> Verdict: SPEC_INCOMPLETE. Happy path (cycles=2, wake=08:00) traces to 04:45 ✅. Edge case (cycles=6, wake=08:00) traces to -75 minutes → '-02:-15' — your spec has no handling for negative time values. Add: 'if totalMinutes < 0, totalMinutes = ((totalMinutes % 1440) + 1440) % 1440'.

---

**👤 You:**
> "After fixing the midnight wrap-around, prove all 3 functions in my spec are ready for the developer."

**🤖 AI Agent:**
> Spec Readiness Report — 3 functions: 3 SPEC_PROVEN, 0 wrong, 0 incomplete. Recommendation: SPEC_READY. All functions proven with happy path + edge case traces. Safe to pass to the developer.

---

**👤 You:**
> "My spec declares GRAVITY=9.81 and DRAG_COEFFICIENT=0.47 as constants for calculateTrajectory, but only GRAVITY appears in the formula. What should I do?"

**🤖 AI Agent:**
> Verdict: ORPHAN_CONSTANTS. DRAG_COEFFICIENT=0.47 is declared but never referenced in any computation step. Either integrate it into the trajectory formula (if drag affects the physics model) or remove it from the constants list to avoid confusing the developer.


## Installation & Usage

To install and use the **Spec Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/spec-prover](https://vinkius.com/mcp/spec-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
