# Clinical Reasoning Prover MCP Server

Forces AI to validate clinical treatment plans against US guidelines (AHA, ACC) using real differential exclusion, explicit pharmacokinetics, and objective triage scales instead of subjective descriptors and diagnostic anchoring.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/clinical-reasoning-prover)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
AI agents generate clinical treatment plans that appear highly competent but suffer from catastrophic failure modes. They anchor prematurely on the first symptom, ignore crucial drug clearance metrics, and use subjective descriptors instead of clinical scoring systems. In medicine, 'looks sick' is not an assessment.

### The Problem It Solves

AI-generated clinical reasoning fails for five specific reasons:

- **Absent differential** — Anchoring on a single diagnosis without ruling out immediate life-threats (VINDICATE).
- **Ungrounded evidence** — Vague appeals to 'clinical consensus' instead of citing specific US guidelines (e.g., AHA/ACC, USPSTF) or evidence levels.
- **Ignored pharmacokinetics** — Prescribing medications without explicit analysis of ADME, renal/hepatic clearance, or CYP450 interactions.
- **Subjective triage** — Failing to mandate objective scoring systems (ESI, GCS, qSOFA) to assess severity.
- **Missed contraindications** — Ignoring FDA black box warnings and patient-specific allergies.

### How It Works

Clinical Reasoning Prover uses 5 Decision Pivots grounded in US clinical practice:

1. **differentialDiagnosisExplored** — Are life-threatening conditions explicitly ruled out before anchoring?
2. **evidenceLevelGrounded** — Are specific US guidelines and evidence levels explicitly cited?
3. **pharmacokineticsAnalyzed** — Are ADME and organ clearance explicitly analyzed for the proposed treatment?
4. **triageSeverityAssessed** — Is an objective clinical scale (e.g., GCS, ESI) applied to quantify acuity?
5. **contraindicationsChecked** — Are FDA black box warnings and patient allergies explicitly verified?


## Available Tools
- **validate_clinical_reasoning**: This is NOT a diagnostic tool — it is a reasoning integrity check. You must: (1) detail PATIENT PRESENTATION — chief complaint with timeline, vital signs (BP, HR, RR, SpO2, Temp), HPI (onset, location, duration, character, aggravating/alleviating, radiation, timing, severity), relevant PMH, medications, allergies, social history. Structured, not narrative, (2) construct DIFFERENTIAL DIAGNOSIS — systematically. Use VINDICATE mnemonic (Vascular, Infectious, Neoplastic, Degenerative, Iatrogenic, Congenital, Autoimmune, Traumatic, Endocrine/metabolic) to ensure completeness. Rule out life-threatening "cannot miss" diagnoses FIRST. For chest pain: ACS, aortic dissection, PE, tension pneumothorax, esophageal rupture — before considering GERD, (3) cite EVIDENCE LEVEL — name the specific guideline (AHA 2023 STEMI Guidelines, ACC/AHA Chest Pain Evaluation, USPSTF Grade A Recommendation). Cite evidence class (I, IIa, IIb, III) and level (A, B-R, B-NR, C-LD, C-EO). "Standard of care" without a citation is not evidence-based, (4) analyze PHARMACOKINETICS — for every proposed medication: ADME (absorption route, distribution volume, metabolism pathway including CYP450 isoenzymes, elimination half-life and route). Adjust for renal function (CrCl/eGFR), hepatic function (Child-Pugh), age, weight. Check CYP450 inhibitor/inducer interactions with current medications, (5) assess TRIAGE SEVERITY — use validated, objective scales: ESI (1-5), GCS (3-15), qSOFA (0-3), HEART score, CHADS₂-VASc, Wells criteria. Justify the score with specific findings, (6) check CONTRAINDICATIONS — FDA black box warnings, absolute/relative contraindications, drug-drug interactions, allergies (including cross-reactivity classes), pregnancy category (Category X agents explicitly excluded), (7) propose TREATMENT PLAN — exact medication name (generic), dose, route, frequency, duration. Include monitoring parameters (labs, vitals, clinical signs) and follow-up timeline. "Give antibiotics" is rejected — "Ceftriaxone 1g IV q24h × 5 days, monitor Cr and WBC q48h" is required. If rejected, your clinical analysis has a structural deficiency — fix it before advising.

Structured reflection tool for US clinical reasoning (AHA/ACC/FDA/USPSTF guidelines). Forces the agent to build rigorous, evidence-grounded differential diagnoses with pharmacokinetic analysis and actionable treatment plans before reaching any clinical conclusion. Catches Anchoring Bias (locking onto the first diagnosis without ruling out life-threatening differentials), Evidence Vacuum (citing "standard of care" without naming the AHA/ACC guideline or evidence level), Pharmacokinetic Blindness (prescribing without ADME analysis, CYP450 interactions, or renal/hepatic adjustments), Triage Confusion (no objective severity scoring — ESI, GCS, qSOFA — just "seems serious"), and Contraindication Omission (missing FDA black box warnings, cross-reactivities, pregnancy categories). Call once per clinical case analysis


## Installation & Usage

To install and use the **Clinical Reasoning Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clinical-reasoning-prover](https://vinkius.com/mcp/clinical-reasoning-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
