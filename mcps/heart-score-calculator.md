# Heart Score Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/heart-score-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/heart-score-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/heart-score-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cardiology](../categories/cardiology.md)

Determine acute myocardial infarction (AMI) risk using five key clinical metrics.

## Description
# Heart Score Calculator: Acute Myocardial Infarction Risk Assessment

The initial assessment of chest pain patients is complex. Determining if symptoms are benign or indicative of a serious cardiac event requires aggregating information from multiple sources--a process prone to human variability and omission.

**The Problem:** Standard clinical pathways require synthesizing data from History, ECGs, Age, Comorbidities (Risk Factors), and Troponin levels into a single, actionable risk score. This synthesis must adhere strictly to AHA/ESC guidelines for immediate patient triage.

**The Mechanism:** This MCP connects AI agents directly to the necessary medical logic using three specialized tools:
1.  `calculate_heart_score`: Aggregates all five components (H, E, A, R, T) into a total score of 0-10.
2.  `classify_risk_and_triage`: Takes the resulting score and maps it to 'Low', 'Moderate', or 'High' risk categories with a defined triage level.
3.  `recommend_clinical_conduct`: Uses the final risk classification to generate mandatory diagnostic pathways, management directives, and follow-up schedules based on current medical standards.

**The Advantage:** The system provides deterministic, guideline-backed clinical decision support. Instead of generic advice, it outputs specific next steps--which tests to order, and where the patient should be managed--allowing clinicians to focus immediately on high-priority care.


## Available Tools
- **calculate_heart_score**: History and ECG scores are optional and default to 0 if not provided.

Calculate the total HEART score for acute myocardial infarction risk assessment
- **classify_risk_and_triage**: Patient age group is optional for validation.

Classify a HEART score into risk category and determine triage priority
- **recommend_clinical_conduct**: Adjusts for emergency room setting and patient gender when provided.

Provide evidence-based clinical recommendations based on risk classification


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Heart Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Patient profile: Age 68, History score 2 (Anginal at rest), ECG score 1 (T-wave inversion), Risk Factor score 2 (Diabetes/Hypertension). Troponin is mildly elevated. Calculate the HEART score and recommend initial conduct."

**🤖 AI Agent:**
> First, I will use `calculate_heart_score` with inputs: historyScore=2, ecgFindingsScore=1, ageFactorScore=2, riskFactorComorbidityScore=2, troponinSeverityScore=1. The total score is 8. Next, using `classify_risk_and_triage(totalScore=8)`, the result is 'High Risk' with Triage Level 3. Finally, I call `recommend_clinical_conduct('High Risk')` which mandates immediate admission and urgent investigation.

---

**👤 You:**
> "I have a young patient (Age 35) with minimal symptoms. My calculated HEART score is 2. What should the next steps be?"

**🤖 AI Agent:**
> The `classify_risk_and_triage` tool confirms a 'Low Risk' status for a total score of 2. Therefore, I run `recommend_clinical_conduct('Low Risk', false)` to get the recommended pathway. The output will guide us toward outpatient follow-up and discharge protocols.

---

**👤 You:**
> "Run a full assessment for an 85-year-old male presenting in the ER. Scores are: History=1, ECG=0, Age=2, RF=1, Troponin=0."

**🤖 AI Agent:**
> Initial calculation via `calculate_heart_score` yields a total score of 4. Using the `classify_risk_and_triage(totalScore=4, patientAgeGroup='over 80')` tool confirms 'Moderate Risk' with Triage Level 2. I then use `recommend_clinical_conduct('Moderate Risk', true, true)` to get actionable ER guidelines.


## Installation & Usage

To install and use the **Heart Score Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/heart-score-calculator](https://vinkius.com/mcp/heart-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
