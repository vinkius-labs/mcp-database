# CHA₂DS₂-VASc & HAS-BLED Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cha2ds2-vasc-has-bled-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cha2ds2-vasc-has-bled-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cha2ds2-vasc-has-bled-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [risk-assessment](../categories/risk-assessment.md)

Calculate stroke risk (CHA₂DS₂-VASc) and bleeding risk (HAS-BLED) for atrial fibrillation patients using established clinical guidelines.

## Description
# Atrial Fibrillation Risk Assessment

The diagnosis of Atrial Fibrillation (AFib) requires careful risk stratification to determine the appropriate balance between preventing stroke and avoiding excessive bleeding. Simply calculating a score is not enough; clinicians need integrated guidance.

**The Problem:** Traditional assessment methods often evaluate thromboembolic risk and hemorrhagic risk separately, leading to disjointed treatment plans. A patient with high AFib risk but also high bleeding risk needs nuanced advice that weighs both factors simultaneously.

**Our Mechanism (Tools):** This MCP connector provides a three-step workflow using specialized tools:
1. **`query_cha2ds2_vasc_score`**: Calculates the total CHA₂DS₂-VASc score based on patient demographics and comorbidities (sex, age, HTN, DM, etc.).
2. **`calculate_hasbled_score`**: Assesses the bleeding risk using the HAS-BLED scale, considering factors like blood pressure control and diuretic use.
3. **`get_risk_recommendations`**: Takes both scores to generate a final recommendation, providing the annual stroke risk percentage (based on ESC 2020 criteria) and definitive anticoagulant guidance ('O' or 'A').

**Advantage:** By running these tools together, agents can provide comprehensive patient care pathways. Instead of just listing a score, they deliver actionable advice that synthesizes both high thromboembolic risk *and* high bleeding risk concerns, guiding the clinician toward optimal therapy.


## Available Tools
- **query_cha2ds2_vasc_score**: Calculate the CHA2DS2-VASc score for atrial fibrillation stroke risk assessment
- **calculate_hasbled_score**: Calculate the HAS-BLED score for bleeding risk assessment during anticoagulation
- **get_risk_recommendations**: Get clinical recommendations based on CHA2DS2-VASc and HAS-BLED scores


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CHA₂DS₂-VASc & HAS-BLED Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Run the full risk assessment. Patient is a 78-year-old male, has HTN and DM. No history of stroke/TIA, but does have documented vascular disease and ICC factor. His BP is 140/90; he takes diuretics and has no GI bleeding history. Recommend anticoagulation."

**🤖 AI Agent:**
> First, we calculate the base risk using **`query_cha2ds2_vasc_score`** (inputs: Male, 78, False, True, True, False, True, True). Next, we assess bleeding risk with **`calculate_hasbled_score`** (inputs: 140, True, False, YES). Finally, **`get_risk_recommendations`** synthesizes these scores, providing the annual stroke risk and the definitive anticoagulation recommendation.

---

**👤 You:**
> "I need to know the bleeding risk for a low-risk patient who is only 65 years old, female, and not taking anticoagulation."

**🤖 AI Agent:**
> We will first run **`query_cha2ds2_vasc_score`** (inputs: Female, 65, False, False, False, False, False, False) to establish the baseline score. Then, we use **`calculate_hasbled_score`** (inputs: Current BP, False, False, NO). The results will guide us on whether further tools are necessary.

---

**👤 You:**
> "What is the overall recommendation for a high-risk patient? Inputs: Male, 85, True (Stroke/TIA), True (HTN), True (DM), False (CHF), True (VascD), True (ICC). BP: 160/95. Diuretic use: Yes. GI Bleeding: No. Anticoagulation Status: YES."

**🤖 AI Agent:**
> The full assessment requires three steps: 1) **`query_cha2ds2_vasc_score`** for the high thromboembolic risk. 2) **`calculate_hasbled_score`** to check bleeding risk (inputs: 160, True, False, YES). 3) **`get_risk_recommendations`** uses both results to give a definitive O/A recommendation and annual stroke percentage.


## Installation & Usage

To install and use the **CHA₂DS₂-VASc & HAS-BLED Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cha2ds2-vasc-has-bled-calculator](https://vinkius.com/mcp/cha2ds2-vasc-has-bled-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
