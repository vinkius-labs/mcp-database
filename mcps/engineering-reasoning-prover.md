# Engineering Reasoning Prover MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/engineering-reasoning-prover)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/engineering-reasoning-prover-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/engineering-reasoning-prover-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

An engineering report cited 'industry standards' without naming a single one. Engineering Reasoning Prover forces ISO/ASME/IEC-grounded compliance analysis — real calculations, real codes, real risk quantification.

## Description
AI agents produce engineering assessments that sound authoritative but collapse under scrutiny. They cite 'industry standards' without naming them. They declare designs 'adequate' without showing calculations. They claim 'compliance' without tracing a single requirement to evidence.

### The Problem It Solves

AI-generated engineering reasoning fails for five specific reasons:

- **Standard misapplication** — Cites a standard but applies the wrong clause, wrong edition, or wrong standard entirely. 'Per ASME' is not a standard reference — 'ASME BPVC Section VIII, Div. 1, UG-27, 2023 Ed.' is.
- **Calculation gap** — Conclusions without verifiable math. 'The design is adequate' without stress analysis, load calculations, or safety factor verification is engineering theater.
- **Code blindness** — Ignores which code governs, which edition is in force, and which authority has jurisdiction. A pressure vessel in Texas has different requirements than one in Germany.
- **Risk hand-waving** — Identifies hazards without quantifying severity, likelihood, or demonstrating mitigation effectiveness. 'Risks have been mitigated' is not a risk assessment.
- **Compliance theater** — Claims compliance without tracing requirements to design evidence. 'Fully compliant' without a requirement-to-evidence matrix proves nothing.

### Key Benefits

- **Forces real standard citations** — Every reference must include exact designation, clause number, and edition year. No more 'per industry standards.'
- **Demands calculation evidence** — Inputs, method, results, acceptance criteria, and safety margin must all be verifiable and traceable.
- **Requires jurisdiction specificity** — Which code, which edition, which AHJ, which local amendments. Engineering varies by jurisdiction.
- **Quantifies risk systematically** — HAZOP, FMEA, or FTA with severity classification, likelihood estimation, and residual risk determination.
- **Traces compliance to evidence** — Requirement-to-evidence matrix mapping each code requirement to the design feature and test that satisfies it.

### Engineering Framework Coverage

- **ISO 9001 / 14001 / 45001** — Quality, Environment, Safety Management
- **IEC 61508 / ISO 26262 / DO-178C** — Functional Safety
- **ASME BPVC / API Standards** — Pressure Equipment
- **IEEE Standards** — Electrical and Software Engineering
- **Eurocodes / ACI / AISC** — Structural Engineering
- **OSHA 29 CFR / EU Machinery Directive** — Workplace Safety
- **NFPA / IBC / NEC** — Fire, Building, Electrical Codes


## Available Tools
- **validate_engineering_reasoning**: Engineering is not intuition — it is standards compliance, quantified risk, and mathematical proof. You must: (1) identify the governing STANDARD — exact designation, clause, edition. "ASME BPVC Section VIII, Div. 1, UG-27, 2023 Ed." is a reference. "Per ASME" is not. Multiple standards may apply — list each with scope, (2) provide CALCULATION evidence — inputs with units and sources, method or formula, numerical results, acceptance criteria from the standard, safety factor or margin. "The design is adequate" is not a calculation, (3) specify CODE and jurisdiction — which code governs, which edition is in force, which authority has jurisdiction (AHJ), which local amendments apply, (4) QUANTIFY risks — hazard identification method (HAZOP, FMEA, FTA), severity classification, likelihood estimation with basis, specific mitigation measures, residual risk after mitigation, (5) TRACE compliance — requirement-to-evidence matrix. For each requirement: the requirement ID, the design feature satisfying it, the analysis or test demonstrating compliance, and the acceptance criterion with actual result. If rejected, your engineering analysis has a structural deficiency.

Structured reflection tool for engineering reasoning and regulatory compliance. Forces the agent to construct rigorous, standards-grounded engineering arguments before any design conclusion. Catches Standard Misapplication (citing "ASME" without specifying BPVC Section VIII Division 1 UG-27 2023 Edition — a 600-page standard is not a reference. The specific clause that governs YOUR design is the reference), Calculation Gap ("the design is adequate" without showing inputs, method, numerical results, acceptance criteria, and safety margin. Engineering is mathematics, not opinion), Code Blindness ("per industry standards" instead of naming the code, edition, jurisdiction, and authority having jurisdiction — codes exist because people died. Cite them), Unquantified Risk ("risks are acceptable" without hazard identification method (HAZOP/FMEA/FTA), severity classification (SIL/ASIL/RPN), likelihood with basis, mitigation measures, and residual risk after mitigation), and Compliance Theater (claiming compliance without a requirement-to-evidence traceability matrix — each requirement mapped to the specific design feature, analysis, or test that satisfies it). Call once per engineering analysis or compliance assessment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Engineering Reasoning Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We need a carbon steel pressure vessel for 450°F service at 600 psig. Verify it meets code requirements."

**🤖 AI Agent:**
> STANDARD_MISAPPLIED — 'meets code requirements' without naming the code. Which code governs? ASME BPVC Section VIII Div. 1 or Div. 2? Which edition? Who is the AHJ? What material spec (SA-516 Gr. 70)? Calculate required thickness per UG-27 with corrosion allowance before claiming compliance.

---

**👤 You:**
> "Evaluate the SIL rating for the emergency shutdown valve on the reactor feed line. The HAZOP identified loss of containment as a consequence."

**🤖 AI Agent:**
> COMPLIANCE_PROVEN — SIL 2 per IEC 61508:2010 with SIF architecture 1oo2, PFDavg = 3.2×10⁻³ within SIL 2 range (10⁻² to 10⁻³), proof test interval 12 months, diagnostic coverage 92%. Risk graph per IEC 61511 confirms SIL 2 target. Compliance traced through SRS to validated test results.

---

**👤 You:**
> "The building structural design uses steel moment frames. Verify seismic compliance for a site in Los Angeles."

**🤖 AI Agent:**
> CALCULATION_GAP — Seismic design for LA (Seismic Design Category D/E) requires specific calculations: site class per ASCE 7-22 Ch. 11, spectral accelerations Ss and S1 from USGS, response modification R for SMF (R=8), drift limits per ASCE 7-22 §12.12. Show the base shear calculation V = CsW.


## Installation & Usage

To install and use the **Engineering Reasoning Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/engineering-reasoning-prover](https://vinkius.com/mcp/engineering-reasoning-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
