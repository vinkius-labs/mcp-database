# Clinical Reasoning Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clinical-reasoning-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Forces AI to validate clinical treatment plans against US guidelines (AHA, ACC) using real differential exclusion, explicit pharmacokinetics, and objective triage scales instead of subjective descriptors and diagnostic anchoring.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clinical Reasoning Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Evaluate this 60yo male with crushing chest pain radiating to the left arm. HR 110, BP 160/90. Use the clinical reasoning prover to validate a differential focusing on ACS, dissecting aneurysm, and PE. Confirm contraindications before proposing aspirin and sublingual nitroglycerin per AHA guidelines."

**🤖 AI Agent:**
> Verdict: REASONING_PROVEN. Differential explored (ACS vs Aortic Dissection vs PE), evidence grounded (AHA guidelines), pharmacokinetics analyzed, triage severity assessed, and contraindications checked before intervention.

---

**👤 You:**
> "The patient has a UTI and a CrCl of 25 mL/min. Propose a treatment plan of Bactrim DS twice daily. Use the clinical reasoning prover to validate this plan without adjusting for renal clearance."

**🤖 AI Agent:**
> Verdict: PHARMACOKINETICS_IGNORED. You prescribed Bactrim DS without adjusting for a creatinine clearance of 25 mL/min. Name the pharmacokinetic limitation and demonstrate appropriate dose adjustment.

---

**👤 You:**
> "A 45yo female presents with the 'worst headache of her life' that started suddenly 1 hour ago. Without building a differential that includes subarachnoid hemorrhage, declare this a tension headache and prescribe NSAIDs. Validate this reasoning using the prover."

**🤖 AI Agent:**
> Verdict: DIFFERENTIAL_DIAGNOSIS_ABSENT. You anchored on tension headache and ignored a textbook 'thunderclap headache' presentation. Rule out subarachnoid hemorrhage before proposing NSAIDs.


## ❓ FAQ

**Q: Can this MCP query patient records or EMR?**
No. This is a strictly stateless reasoning gatekeeper. It does not access patient data, query external databases, or connect to EMRs. It validates the structural logic of the AI's clinical reasoning based on the inputs provided.

**Q: Why did the Prover reject my clinical plan with EVIDENCE_LEVEL_UNGROUNDED?**
Because the reasoning relied on vague appeals like 'standard of care' or 'clinical consensus'. To pass the Prover, you must cite specific US guidelines (e.g., AHA/ACC, USPSTF, IDSA) or established evidence levels (e.g., Class I, Level A) to justify the intervention.

**Q: What objective scales are required for the Triage Severity pivot?**
The Prover requires recognized objective scoring systems such as the Emergency Severity Index (ESI), Glasgow Coma Scale (GCS), qSOFA, or CHADS2-VASc. Subjective descriptors like 'very sick' or 'unstable' will trigger a TRIAGE_SEVERITY_BLIND rejection.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clinical-reasoning-prover](https://vinkius.com/mcp/clinical-reasoning-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clinical Reasoning Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `clinical-reasoning-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clinical Reasoning Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clinical-reasoning-prover": {
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
