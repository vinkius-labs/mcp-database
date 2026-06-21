# Curie Measurement Prover MCP Server

A team shipped a 'significant performance improvement.' Workflow, supplier, automation, and schedule all changed at once. Processing time dropped — but nobody knew which change helped most. The automation alone accounted for 89% of the gain. The supplier switch introduced a defect that surfaced 72 hours later. Curie processed 8 tons of pitchblende to isolate 0.1 grams of radium — ONE element at a time. This tool forces that discipline: measure with numbers, isolate variables, validate across environments, persist through investigation, and quantify risks.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/curie-measurement-prover)

## Overview
**Category:** complex-reasoning
**Tools Count:** 1

## Description
Agents say 'faster' without benchmarks, 'more reliable' without error rates, 'improved' without measurements. They change five things at once and call it an improvement. They test only in one context and call it validated.

### The Problem

LLMs commit five empirical failures:

- **Measurement Absent** — 'The new process is significantly faster.' Curie did not say 'more radioactive.' She measured the activity of radium at 2 million times that of uranium, using an electrometer she and Pierre built specifically for the task. Where is YOUR number? What is the baseline? The after-value? The delta?
- **Isolation Incomplete** — 'We changed the supplier, the workflow, and the schedule, and performance improved.' Curie separated pitchblende into chemical fractions and measured the radioactivity of EACH fraction individually. She did not test the whole rock. When you change 3 things at once, which one helped? Which one introduced the defect that appears 72 hours later?
- **Cross-Domain Unvalidated** — 'Works in our department.' Curie won the Nobel Prize in Physics (1903) AND Chemistry (1911) — the only person in history to win in two different sciences. Her measurements were reproducible in every laboratory in Europe, not just her converted Parisian shed. Have you tested in other conditions? Under peak demand? With real-world data?
- **Persistence Insufficient** — 'We tried and it does not work.' Curie processed 8 TONS of pitchblende over 4 years — in a shed with a leaking roof, self-funded, facing systematic discrimination as a woman in 1900s academia — to isolate 0.1 grams of radium chloride. How many attempts did you make? With what systematic variations?
- **Risk Unquantified** — 'The risk is minimal.' Curie died of aplastic anemia from radiation exposure. Her personal notebooks from the 1890s are STILL radioactive — stored in lead-lined boxes at the Bibliothèque nationale de France, requiring protective clothing to handle. She documented radioactivity but failed to quantify her own risk. What are YOUR risks? With what probability? What impact? What mitigation?

### How It Works

5 Decision Pivots following Curie's methodology:

1. **measurementRigorous** — Baseline, method, after-value, quantified delta.
2. **isolationComplete** — Single variable, controls maintained, attribution proven.
3. **crossDomainValidated** — Multiple environments, conditions, data sets.
4. **persistenceDocumented** — Duration, attempts with results, systematic approach.
5. **riskQuantified** — Each danger with probability, impact, mitigation.

### The Verdict Matrix

| First Failing Pivot | Verdict | Meaning |
|---|---|---|
| measurementRigorous = false | MEASUREMENT_ABSENT | Adjectives instead of numbers. |
| isolationComplete = false | ISOLATION_INCOMPLETE | Multiple variables changed. |
| crossDomainValidated = false | CROSS_DOMAIN_UNVALIDATED | Tested in one environment only. |
| persistenceDocumented = false | PERSISTENCE_INSUFFICIENT | Abandoned prematurely. |
| riskQuantified = false | RISK_UNQUANTIFIED | Dangers dismissed without data. |
| All pivots pass | MEASUREMENT_PROVEN | Measured. Isolated. Validated. Persisted. Risk-aware. |


## Available Tools
- **validate_curie_measurement**: Think like Marie Curie — who measured what others said could not be measured, isolated variables across thousands of fractions, validated across two entire sciences, persisted for 4 years on a single extraction, and understood risk so well that her notebooks still require lead-lined boxes. You must: (1) MEASURE — specify baseline (current measured value), method (instrument/process), after-value (measured result), and delta (quantified change with percentage). "Significantly better," "improved performance," and "notable improvement" are not measurements, (2) ISOLATE — change ONE variable, control everything else, prove attribution (reversing restores the old result), and verify reproducibility (repeat the experiment, measure variance). "We redesigned the process" is correlation, not causation. Curie tested ONE element at a time, (3) CROSS-VALIDATE — test in multiple contexts (locations, user segments, time periods), under multiple conditions (low demand, peak, stressed, degraded), with multiple data sets (small sample, full population, edge cases). A result that only works in one context is a coincidence, (4) PERSIST — document systematic investigation with specific attempts, measured results per attempt, and duration. "We tried and it failed" after 2 attempts is premature abandonment. Curie: 4 years, 8 tons of pitchblende, 0.1 grams of radium, (5) QUANTIFY RISK — each danger with probability (based on historical data or structured estimation), impact (in currency, time, or scope), and mitigation strategy. "The risk is minimal" is not quantification. If rejected, your claim lacks empirical foundation.

Structured reflection tool for Marie Curie-level empirical rigor — replacing qualitative claims with quantitative measurements, isolating variables, cross-validating across contexts, persisting through systematic investigation, and quantifying risks with probability and impact. Catches Measurement Absence ("significantly better" without baseline, method, after-value, and delta — Curie measured radioactivity when others said it was unmeasurable), Isolation Failure (changing 3 variables at once and claiming causation — "we redesigned the process and results improved" without isolating which change drove improvement), Single-Context Validation ("it worked in one test" without varying conditions, populations, scales, or environments — Curie won Nobel Prizes in Physics AND Chemistry, not one lab), Persistence Deficit ("we tried and it failed" after 2 attempts instead of systematic investigation — Curie: 4 years, 8 tons of pitchblende, 0.1 grams of radium), and Risk Handwaving ("the risk is minimal" without probability, impact, and mitigation for each danger — Curie's notebooks are still radioactive after 120 years). Call once per empirical claim, performance assertion, or data-driven recommendation


## Installation & Usage

To install and use the **Curie Measurement Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/curie-measurement-prover](https://vinkius.com/mcp/curie-measurement-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
