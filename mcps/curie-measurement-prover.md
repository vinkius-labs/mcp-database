# Curie Measurement Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/curie-measurement-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [complex-reasoning](../categories/complex-reasoning.md)

A team shipped a 'significant performance improvement.' Workflow, supplier, automation, and schedule all changed at once. Processing time dropped — but nobody knew which change helped most. The automation alone accounted for 89% of the gain. The supplier switch introduced a defect that surfaced 72 hours later. Curie processed 8 tons of pitchblende to isolate 0.1 grams of radium — ONE element at a time. This tool forces that discipline: measure with numbers, isolate variables, validate across environments, persist through investigation, and quantify risks.

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


## Available Tools (1)
- **validate_curie_measurement**: Think like Marie Curie — who measured what others said could not be measured, isolated variables across thousands of fractions, validated across two entire sciences, persisted for 4 years on a single extraction, and understood risk so well that her notebooks still require lead-lined boxes. You must: (1) MEASURE — specify baseline (current measured value), method (instrument/process), after-value (measured result), and delta (quantified change with percentage). "Significantly better," "improved performance," and "notable improvement" are not measurements, (2) ISOLATE — change ONE variable, control everything else, prove attribution (reversing restores the old result), and verify reproducibility (repeat the experiment, measure variance). "We redesigned the process" is correlation, not causation. Curie tested ONE element at a time, (3) CROSS-VALIDATE — test in multiple contexts (locations, user segments, time periods), under multiple conditions (low demand, peak, stressed, degraded), with multiple data sets (small sample, full population, edge cases). A result that only works in one context is a coincidence, (4) PERSIST — document systematic investigation with specific attempts, measured results per attempt, and duration. "We tried and it failed" after 2 attempts is premature abandonment. Curie: 4 years, 8 tons of pitchblende, 0.1 grams of radium, (5) QUANTIFY RISK — each danger with probability (based on historical data or structured estimation), impact (in currency, time, or scope), and mitigation strategy. "The risk is minimal" is not quantification. If rejected, your claim lacks empirical foundation.

Structured reflection tool for Marie Curie-level empirical rigor — replacing qualitative claims with quantitative measurements, isolating variables, cross-validating across contexts, persisting through systematic investigation, and quantifying risks with probability and impact. Catches Measurement Absence ("significantly better" without baseline, method, after-value, and delta — Curie measured radioactivity when others said it was unmeasurable), Isolation Failure (changing 3 variables at once and claiming causation — "we redesigned the process and results improved" without isolating which change drove improvement), Single-Context Validation ("it worked in one test" without varying conditions, populations, scales, or environments — Curie won Nobel Prizes in Physics AND Chemistry, not one lab), Persistence Deficit ("we tried and it failed" after 2 attempts instead of systematic investigation — Curie: 4 years, 8 tons of pitchblende, 0.1 grams of radium), and Risk Handwaving ("the risk is minimal" without probability, impact, and mitigation for each danger — Curie's notebooks are still radioactive after 120 years). Call once per empirical claim, performance assertion, or data-driven recommendation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Curie Measurement Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We switched from the old process to the new one and operations feel significantly faster. Performance is greatly improved."

**🤖 AI Agent:**
> MEASUREMENT_ABSENT — 'Feels significantly faster' and 'greatly improved' are adjectives, not measurements. Curie did not say radium 'seems more radioactive' — she measured its activity at 2 million times that of uranium. Where is YOUR baseline? What was the old process cycle time under normal demand? What is the new process cycle time under the same conditions? What is the delta? 'Faster' measured HOW — time study? controlled comparison? subjective impression? Without numbers, you have an opinion, not evidence.

---

**👤 You:**
> "Measurement: Old process baseline: 847 minutes per batch under standard conditions (timed over 5 consecutive batches, same team, same materials). New process: 312 minutes per batch (same team, same materials, same conditions). Delta: 535 minutes reduction (63.2%). BUT — we also changed the raw material supplier and restructured the team schedule in the same transition."

**🤖 AI Agent:**
> ISOLATION_INCOMPLETE — Measurement is rigorous: 847min → 312min, 63.2% reduction, same team and materials. Excellent baseline discipline. But isolation fails: three variables changed simultaneously — new process, new supplier, new schedule. The new supplier alone might have delivered higher-quality inputs requiring less rework. The schedule restructuring might have eliminated bottleneck shift changes. You do not know if the new process contributed 90% of the improvement or 10%. Curie did not test the entire rock — she separated it into fractions. Suggestion: test the new process with the old supplier and old schedule first (isolate process variable), then introduce one change at a time.

---

**👤 You:**
> "Measurement: 847→312min (63.2%). Isolation: tested new process with old supplier and old schedule = 624min. Then new process with new supplier and old schedule = 480min. Then all three changes = 312min. Attribution: process change accounts for 223min (42%), supplier accounts for 144min (27%), schedule accounts for 168min (31%). Reproducible: 3 runs, variance ±8min. Cross-domain: tested in main facility and satellite facility. Peak conditions: not yet tested under peak season demand, we assume it transfers."

**🤖 AI Agent:**
> CROSS_DOMAIN_UNVALIDATED — Measurement and isolation are excellent: 847→312min, process 42%, supplier 27%, schedule 31%, 3 runs with ±8min variance. Rigorous isolation across two facilities. But cross-domain fails: 'not yet tested under peak season demand, we assume it transfers.' Curie's measurements were reproducible in EVERY laboratory in Europe. Normal conditions are NOT peak conditions: peak season has different volumes, different material quality, different team fatigue levels, different equipment utilization rates. Run the new process through one peak season cycle, measure for a full cycle under real conditions, then compare.


## ❓ FAQ

**Q: Is this only for performance optimization?**
No. Curie's method applies to any domain requiring empirical validation — process improvement (measure before/after cycle times, isolate each change), vendor evaluation (measure cost/quality/reliability, not 'it seems better'), risk assessment (quantify probability and impact, not 'the risk is minimal'), method selection (benchmark each candidate in isolation), controlled experiments (single variable, controlled conditions). Anywhere you would say 'better' or 'faster' or 'more reliable,' replace the adjective with a number.

**Q: What if isolation is impractical?**
Sometimes variables are genuinely coupled — changing the supplier requires changing the delivery schedule. The engine does not demand artificial isolation. It demands AWARENESS of what was changed together and WHY isolation was impractical. Document: 'We changed X and Y together because X requires Y. We cannot isolate their effects. We accept that the 67% improvement is from X+Y combined, with Y alone contributing approximately 15% based on a separate controlled test.' Honest documentation of coupled changes is acceptable. Pretending 3 changes are one is not.

**Q: How does it differ from the Watt Efficiency Prover?**
Watt validates EFFICIENCY ENGINEERING — finding waste, instrumenting baselines, designing feedback loops, isolating bottlenecks, quantifying improvements. It asks 'where is the bottleneck?' Curie validates EMPIRICAL RIGOR — measuring instead of claiming, isolating variables, cross-domain validation, persistence, risk quantification. It asks 'where is the number?' Watt finds WHERE to optimize. Curie proves THAT you optimized. Use Watt to identify bottlenecks. Use Curie to prove your fix actually worked — with numbers, not adjectives.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/curie-measurement-prover](https://vinkius.com/mcp/curie-measurement-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Curie Measurement Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `curie-measurement-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Curie Measurement Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "curie-measurement-prover": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
