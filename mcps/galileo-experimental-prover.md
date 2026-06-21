# Galileo Experimental Prover MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/galileo-experimental-prover)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/galileo-experimental-prover-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/galileo-experimental-prover-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [architecture](../categories/architecture.md)

Your AI accepted a claim because 'the documentation recommends it.' That is authority deference — not evidence. Galileo did not accept Aristotle's 2,000-year claim that heavier objects fall faster. He dropped two masses from the Tower of Pisa. This tool forces authority questioning, experimental design, variable control, outcome prediction, and belief revision.

## Description
AI agents accept claims from authority. 'The vendor says,' 'the industry standard,' 'best practice dictates.' They never design an experiment to test the claim.

### The Problem

- **Authority Deferred** — 'Use this because the documentation recommends it.' Galileo dropped two masses from the Tower of Pisa to disprove Aristotle.
- **Experiment Absent** — 'It stands to reason.' Galileo built a 20x telescope and SHOWED Jupiter's moons.
- **Variables Uncontrolled** — 'We changed the process, tools, and team — results improved.' Which change mattered? Galileo varied ONLY the angle.
- **Prediction Missing** — 'Let us see what happens.' Galileo PREDICTED equal fall rates BEFORE testing.
- **Dogma Persistent** — 'The data is anomalous.' The Aristotelians REFUSED to look through the telescope.

### How It Works

1. **authorityQuestioned** — Claim challenged at its source. Evidence, not prestige.
2. **experimentDesigned** — Specific, repeatable test with hypothesis and measurement.
3. **variablesControlled** — Only ONE variable changes. Everything else constant.
4. **outcomePredicted** — Expected result stated BEFORE the experiment.
5. **beliefRevised** — Position updated when evidence contradicts.

### Verdict Matrix

| Pivot | Verdict | Meaning |
|---|---|---|
| authorityQuestioned = false | AUTHORITY_DEFERRED | Claim accepted by prestige. |
| experimentDesigned = false | EXPERIMENT_ABSENT | No test designed. |
| variablesControlled = false | VARIABLES_UNCONTROLLED | Multiple changes, no attribution. |
| outcomePredicted = false | PREDICTION_MISSING | No prediction before test. |
| beliefRevised = false | DOGMA_PERSISTENT | Evidence contradicts, position unchanged. |
| All pass | EXPERIMENT_PROVEN | Full experimental method. |


## Available Tools
- **validate_galileo_experiment**: Galileo did not accept 2,000 years of Aristotelian physics — he tested it. You must: (1) QUESTION AUTHORITY — challenge the claim at its source. Evaluate evidence, not prestige. "The documentation says" is a starting hypothesis, not proof. "I tested the documented behavior and confirmed/denied it" is evidence, (2) DESIGN an EXPERIMENT — create a specific, repeatable test with hypothesis, method, measurement instrument, and repeatability protocol. Galileo built his own telescope and water clock because existing instruments were inadequate, (3) CONTROL VARIABLES — change ONLY ONE variable, hold everything else constant. If you change two things and the result improves, you do not know which caused it, (4) PREDICT OUTCOME before testing — state what you expect, what confirms, what denies, and what single result would FALSIFY the hypothesis entirely. Without a prediction, any result confirms bias, (5) REVISE BELIEFS when evidence contradicts them — update your position, do not dismiss the data. The Aristotelians refused to look through the telescope. Do not be them. If rejected, your reasoning is faith-based, not evidence-based.

Structured reflection tool for Galileo-level experimental reasoning — forces questioning authority with evidence (not prestige), designing controlled experiments with measurable predictions, isolating single variables, stating predictions BEFORE testing, and revising beliefs when evidence contradicts them. Catches Authority Deferred (accepting a claim because of WHO said it instead of WHAT evidence supports it — "the vendor whitepaper says 10x performance" is deference. "I benchmarked the vendor's tool against our current solution on our production dataset and measured 2.3x improvement, not 10x" is evidence. Galileo did not accept Aristotle's 2,000-year-old claim that heavy objects fall faster — he dropped two masses from Pisa and measured), Experiment Absent (proposing solutions without testing them — "it stands to reason" is not evidence. A specific hypothesis, a defined method, a measurement instrument with known precision, and a repeatable protocol IS an experiment. Galileo built his own 20x telescope and water clock to 1/100th second precision because existing instruments were not accurate enough), Variables Uncontrolled (changing multiple things at once and attributing results to one — "we deployed the new code AND upgraded the database AND added caching, and performance improved." Which change caused the improvement? Galileo's inclined plane: changed ONLY the angle, same ball, same surface, same timing), Prediction Missing ("let us see what happens" instead of stating the expected outcome BEFORE running the test — without a prediction, any result confirms your hypothesis. Galileo predicted equal fall rates BEFORE dropping the masses), and Dogma Persistent (dismissing contradicting evidence as "anomalous" instead of updating beliefs — the Aristotelians REFUSED to look through Galileo's telescope because the evidence would challenge their worldview. Do not refuse to look through the telescope). Call once per claim validation, A/B test, or experimental design


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Galileo Experimental Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We should switch to the new process because the vendor documentation says it handles higher volumes and three major companies adopted it."

**🤖 AI Agent:**
> AUTHORITY_DEFERRED — 'The vendor documentation says' and 'three companies adopted it' are authority deference. Galileo did not accept Aristotle because every university taught it. He dropped two masses. At what volume does YOUR current process fail? What experiment would disprove the vendor's claim?

---

**👤 You:**
> "Authority challenged: vendor claims 40% improvement at 10,000 items/day but we process 850. Experiment: 10%/90% split test, 14 days, same items and team. Variables: ONLY routing changes. Prediction: time drops from 34 to ~20 min/item if true, stays 30-34 if false. Revision: abandon if no improvement — evidence outweighs authority."

**🤖 AI Agent:**
> EXPERIMENT_PROVEN — Galilean method complete. Authority challenged at source. Experiment designed with split test. Variables controlled. Outcome predicted with threshold. Belief revision committed.

---

**👤 You:**
> "Authority challenged: manager says Monday meetings are essential. Experiment: removed meetings for two weeks and also changed the reporting tool and moved to daily written updates. Results improved."

**🤖 AI Agent:**
> VARIABLES_UNCONTROLLED — Three things changed simultaneously: removed meetings, changed tool, added written updates. Which caused the improvement? Galileo varied ONLY the angle — same ball, same surface, same timing. Change ONE variable at a time.


## Installation & Usage

To install and use the **Galileo Experimental Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/galileo-experimental-prover](https://vinkius.com/mcp/galileo-experimental-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
