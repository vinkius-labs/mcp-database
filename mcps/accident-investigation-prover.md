# Accident Investigation Prover MCP Server

An investigation report concluded 'pilot error' and recommended 'improve training.' The same airline had three more accidents in 18 months. Accident Investigation Prover forces ICAO Annex 13 methodology — FDR/CVR evidence chains, multi-causal analysis via Reason's Model, HFACS 4-level taxonomy, organizational factor tracing, and specific, measurable, addressed recommendations that prevent recurrence.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/accident-investigation-prover)

## Overview
**Category:** safety & compliance
**Tools Count:** 1

## Description
Accident Investigation Prover enforces NTSB/ICAO Annex 13 investigation rigor across 5 axes that LLMs consistently fail:

**Axis 1 — Evidence Chain.** Narrative-based 'it appears that' is rejected. Every conclusion must be supported by FDR parameters (88 minimum per ICAO Annex 6), CVR transcript with timestamps, ATC recordings correlated with radar track, maintenance logs (MEL items, AD compliance, component life limits), and wreckage analysis (fracture type: fatigue vs overload).

**Axis 2 — Causal Chain.** Single-cause 'the accident was caused by pilot error' is rejected. NTSB format: 'The probable cause was [X], contributing to which were [Y, Z, W].' Reason's Model: latent conditions + active failures + inadequate defenses. 5-Whys to trace systemic root causes.

**Axis 3 — HFACS Taxonomy.** Unclassified 'human error' is rejected. Every factor must be classified across 4 levels: Level 1 (Unsafe Acts — errors and violations), Level 2 (Preconditions — environment, individual condition, CRM), Level 3 (Unsafe Supervision — inadequate, planned inappropriate, failed to correct), Level 4 (Organizational — resources, climate, process). If all factors cluster at Level 1, the investigation is not deep enough.

**Axis 4 — Organizational Factors.** 'The pilot should have' is rejected. Scheduling pressure (utilization rates, FDP violations), training adequacy (budget, syllabus coverage), maintenance economics (MEL deferral rates), regulatory environment (audit frequency), and financial pressure are mandatory analysis targets.

**Axis 5 — Recommendation Actionability.** 'Improve training' is rejected. Every recommendation must be: Specific (what action), Measurable (success criteria), Addressed (to named authority), Tracked (follow-up timeline), Evidence-linked (to which finding).

ICAO Annex 13, 3.1: 'The sole objective shall be the prevention of accidents. It is NOT the purpose to apportion blame or liability.'


## Available Tools
- **validate_accident_investigation**: Before reaching any investigation conclusion, call this tool. You must: (1) CORRELATE EVIDENCE — FDR 88 parameters with timestamps, CVR transcript correlation, ATC radar track and clearances, maintenance logs (MEL, AD compliance, component TSN/TSO), wreckage analysis (fracture type: fatigue vs overload, fire pattern, impact signatures). Cross-reference ALL sources — narrative without data is speculation, (2) CONSTRUCT CAUSAL CHAIN — probable cause + contributing factors (NTSB format: "Probable cause was [X], contributing to which were [Y, Z, W]"). Apply 5-Whys to reach systemic causes. Map to Reason's Model: latent conditions + active failures + defense gaps, (3) CLASSIFY via HFACS — every factor at its correct level: Level 1 (unsafe acts: decision/skill/perceptual errors, routine/exceptional violations), Level 2 (preconditions: environment, individual condition, CRM), Level 3 (supervision: inadequate, planned inappropriate, failed to correct, supervisory violations), Level 4 (organizational: resources, climate, process). If all factors cluster at Level 1, you have not investigated deeply enough, (4) ANALYZE ORGANIZATIONAL factors — scheduling pressure, training budget, maintenance economics, regulatory oversight gaps, financial pressure on safety decisions. The pilot is the LAST link in a chain that starts with organizational decisions months or years before, (5) WRITE ACTIONABLE RECOMMENDATIONS — specific (what action), measurable (success criteria), addressed (to named authority), tracked (response timeline + verification), evidence-linked (to which finding). "Improve training" is a wish — not a recommendation. If rejected, your investigation has a structural deficiency — deepen the analysis.

Structured reflection tool for ICAO Annex 13/NTSB-standard accident investigation. Forces the agent to construct multi-causal, evidence-correlated, taxonomy-classified investigation analyses before reaching any conclusion. Catches Evidence Gaps (narrative without FDR/CVR cross-reference), Single Cause Fallacy (blaming one factor instead of Reason's Swiss Cheese Model), HFACS Blindness (labeling "human error" without 4-level taxonomy classification), Organizational Amnesia (ignoring scheduling, training, maintenance, and regulatory systemic pressures), and Recommendation Theater (vague "improve training" instead of specific, measurable, addressed, tracked, evidence-linked actions). Call once per investigation analysis


## Installation & Usage

To install and use the **Accident Investigation Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/accident-investigation-prover](https://vinkius.com/mcp/accident-investigation-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
